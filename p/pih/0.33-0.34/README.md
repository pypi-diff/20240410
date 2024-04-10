# Comparing `tmp/pih-0.33.tar.gz` & `tmp/pih-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.33.tar", last modified: Tue Apr  2 23:28:02 2024, max compression
+gzip compressed data, was "pih-0.34.tar", last modified: Wed Apr 10 01:57:22 2024, max compression
```

## Comparing `pih-0.33.tar` & `pih-0.34.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 23:28:02.157410 pih-0.33/
--rw-rw-rw-   0        0        0      247 2024-04-02 23:28:02.093831 pih-0.33/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 23:27:59.489820 pih-0.33/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.33/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:28:00.165710 pih-0.33/pih/collections/
--rw-rw-rw-   0        0        0    28133 2024-04-02 01:24:26.000000 pih-0.33/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-02-21 00:45:01.000000 pih-0.33/pih/collections/service.py
--rw-rw-rw-   0        0        0   104106 2024-04-02 01:12:34.000000 pih-0.33/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.33/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:28:01.590188 pih-0.33/pih/consts/
--rw-rw-rw-   0        0        0    25132 2024-04-02 23:24:59.000000 pih-0.33/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3650 2024-03-11 05:53:16.000000 pih-0.33/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1584 2024-03-22 01:07:28.000000 pih-0.33/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.33/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.33/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.33/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29270 2024-03-13 12:22:09.000000 pih-0.33/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.33/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.33/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.33/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.33/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.33/pih/consts/password.py
--rw-rw-rw-   0        0        0    11276 2024-03-29 04:57:29.000000 pih-0.33/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.33/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.33/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.33/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.33/pih/consts/rpc.py
--rw-rw-rw-   0        0        0      924 2024-02-15 03:33:44.000000 pih-0.33/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.33/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.33/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13234 2024-03-26 00:15:02.000000 pih-0.33/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.33/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.33/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   546859 2024-04-02 08:28:41.000000 pih-0.33/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:28:01.794353 pih-0.33/pih/rpc/
--rw-rw-rw-   0        0        0    34084 2024-02-21 13:10:29.000000 pih-0.33/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.33/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.33/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.33/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:28:01.968305 pih-0.33/pih/tools/
--rw-rw-rw-   0        0        0    51249 2024-03-30 01:04:09.000000 pih-0.33/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3958 2024-02-26 05:50:04.000000 pih-0.33/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.33/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:28:02.046938 pih-0.33/pih.egg-info/
--rw-rw-rw-   0        0        0      247 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 23:28:02.173033 pih-0.33/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.595889 pih-0.34/
+-rw-rw-rw-   0        0        0      247 2024-04-10 01:57:22.516696 pih-0.34/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:57:20.337723 pih-0.34/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.34/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:57:20.714803 pih-0.34/pih/collections/
+-rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.34/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.34/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.34/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.34/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.084004 pih-0.34/pih/consts/
+-rw-rw-rw-   0        0        0    25247 2024-04-10 01:56:44.000000 pih-0.34/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.34/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.34/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.34/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.34/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.34/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.34/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.34/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.34/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.34/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.34/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.34/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11359 2024-04-10 01:28:07.000000 pih-0.34/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.34/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.34/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.34/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.34/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.34/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.34/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.34/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.34/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.34/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.34/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   547826 2024-04-09 23:48:44.000000 pih-0.34/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.271491 pih-0.34/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.34/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.34/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.34/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.34/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.381901 pih-0.34/pih/tools/
+-rw-rw-rw-   0        0        0    51367 2024-04-09 22:35:48.000000 pih-0.34/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.34/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.34/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.460022 pih-0.34/pih.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:57:22.595889 pih-0.34/setup.cfg
```

### Comparing `pih-0.33/pih/collections/__init__.py` & `pih-0.34/pih/collections/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1104,20 +1104,21 @@
     title: str | None = None
     text: str | None = None
     parameters: dict[str, Any] | None = None
 
 
 @dataclass
 class BonusInformation:
-    all: float = 0
-    spent: float = 0
-    active: float = 0
-    last_money_spent: float = 0
-    last_spent: float = 0
-    last: float = 0
+    bonus_all: float = 0
+    money_all: float = 0
+    bonus_spent_all: float = 0
+    bonus_active: float = 0
+    money_last: float = 0
+    bonus_last_spent: float = 0
+    bonus_last: float = 0
 
 
 @dataclass
 class WappiStatus:
 
     app_status: str | None = None
     authorized: bool = False
```

### Comparing `pih-0.33/pih/collections/service.py` & `pih-0.34/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/console_api.py` & `pih-0.34/pih/console_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import ipih
 
 from pih import PIH, A, ActionValue, ActionStack, Input, Output, Session
 from pih.consts import (
     FILE,
     PASSWORD,
-    SPLITTER,
     MarkType,
     SessionFlags,
     PasswordSettings,
     CheckableSections,
 )
 from pih.consts.errors import NotFound
 from pih.collections import (
@@ -459,15 +458,15 @@
                                 ).total_seconds()
 
                                 def repr_value(title: str, value: int) -> str:
                                     return js(
                                         (
                                             "",
                                             A.CT_V.BULLET,
-                                            j((title, SPLITTER)),
+                                            j((title, A.CT.SPLITTER)),
                                             self.bold(
                                                 js(
                                                     (
                                                         str(
                                                             int(
                                                                 100
                                                                 * (
@@ -508,15 +507,15 @@
                                 item.default_value
                             )
                             self.output.write_line(
                                 js(
                                     (
                                         "",
                                         A.CT_V.BULLET,
-                                        j((self.bold(item.description), SPLITTER)),
+                                        j((self.bold(item.description), A.CT.SPLITTER)),
                                         j(
                                             (
                                                 nl(
                                                     nl(
                                                         js(
                                                             (
                                                                 "  ",
@@ -2010,15 +2009,15 @@
                     )
                     A.A_M.create(
                         self.full_name,  # type: ignore
                         self.mark_person_division_id,  # type: ignore
                         self.mark_tab_number,
                         self.telephone_number,
                     )
-                if A.A_D.create_for_user(
+                if A.A_DOC.create_for_user(
                     A.PTH_U.get_document_name(
                         A.D.fullname_to_string(self.full_name),  # type: ignore
                         self.login if self.user_is_exists else None,
                     ),
                     self.full_name,  # type: ignore
                     self.mark_tab_number,  # type: ignore
                     LoginPasswordPair(self.login, self.password) if is_user else None,
```

### Comparing `pih-0.33/pih/console_api_wrapper.py` & `pih-0.34/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/__init__.py` & `pih-0.34/pih/consts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.33"
-
-EMAIL_SPLITTER: str = "@"
-ISOLATED_ARG_NAME: str = "isolated"
-ARGUMENT_PREFIX: str = "--"
-SPLITTER: str = ":"
-UNKNOWN: str = "?"
-
+VERSION: str = "0.34"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
@@ -127,19 +120,26 @@
         POWER_SHELL_REMOTE_SESSION: str = "wsmprovhost.exe"
 
     class PORT:
         SMB: int = 445
 
 
 class CONST(DATE_TIME):
+    
+    EMAIL_SPLITTER: str = "@"
+    ISOLATED_ARG_NAME: str = "isolated"
+    ARGUMENT_PREFIX: str = "--"
+    SPLITTER: str = ":"
+    UNKNOWN: str = "?"
 
     class PORT:
         HTTP: int = 80
         SMTP: int = 587
         IMAP: int = 993
+        SNMP: int = 161
 
     class FILES:
         SECTION: str = "Мобильные файлы"
 
     class NOTES:
         SECTION: str = "Мобильные заметки"
 
@@ -493,14 +493,15 @@
         "Запрос к базе данный Polibase (Oracle)",
         "polibase",
         "полибейс",
         "oracle",
     )
     DATA_SOURCE = ("Запрос к базе данных DataSource (DS)", "ds")
     CMD = ("Консольную команду", "cmd")
+    POWERSHELL = ("Powershell команду", "powershell")
     PYTHON = ("Скрипт Python", "py", "python")
     SSH = ("Команда SSH", "ssh")
 
 
 class LogMessageChannels(IntEnum):
     BACKUP = auto()
     POLIBASE = auto()
@@ -638,24 +639,24 @@
         False,
         False,
     )
 
     DOOR_OPEN = ActionDescription(
         "DOOR_OPEN",
         ("door_open",),
-        "Открытие дверей",
+        "Открыть {name} дверь",
         "Открыть",
         False,
         False,
     )
 
     DOOR_CLOSE = ActionDescription(
         "DOOR_CLOSE",
         ("door_close",),
-        "Закрытие дверей",
+        "Закрыть {name} дверь",
         "Закрыть",
         False,
         False,
     )
 
     ATTACH_SHARED_DISKS = ActionDescription(
         "ATTACH_SHARED_DISKS",
```

### Comparing `pih-0.33/pih/consts/ad.py` & `pih-0.34/pih/consts/ad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pih.tools import j
+from pih.tools import j, jp
 from pih.consts.names import USER_PROPERTIES
 
 from enum import Enum, auto
 
 class AD:
     
     ADMINISTRATOR_LOGIN: str = "Administrator"
@@ -45,15 +45,15 @@
         "RESERVED",
         "PARTIAL_SECRETS_ACCOUNT",
     ]
     
     DOMAIN_NAME: str = "fmv"
     DOMAIN_ALIAS: str = "pih"
     DOMAIN_SUFFIX: str = "lan"
-    DOMAIN_DNS: str = j((DOMAIN_NAME, DOMAIN_SUFFIX), SPLITTER)
+    DOMAIN_DNS: str = jp((DOMAIN_NAME, DOMAIN_SUFFIX))
     DOMAIN_MAIN: str = DOMAIN_DNS
     PATH_ROOT: str = j(("//", DOMAIN_MAIN))
 
     ROOT_CONTAINER_DN: str = f"{OU}Unit,DC={DOMAIN_NAME},DC={DOMAIN_SUFFIX}"
     WORKSTATIONS_CONTAINER_DN: str = f"{OU}Workstations,{ROOT_CONTAINER_DN}"
     SERVERS_CONTAINER_DN: str = f"{OU}Servers,{ROOT_CONTAINER_DN}"
     USERS_CONTAINER_DN_SUFFIX: str = f"Users,{ROOT_CONTAINER_DN}"
```

### Comparing `pih-0.33/pih/consts/addresses.py` & `pih-0.34/pih/consts/addresses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pih.tools import j, js, jp
-from pih.consts import EMAIL_SPLITTER, SPLITTER
+from pih.consts import CONST
 
 
 class ADDRESSES:
 
     REMOTE_PREFIX: str = "remote"
     SITE_NAME: str = "pacifichosp"
     SITE_ADDRESS: str = jp((SITE_NAME, "com"))
@@ -17,27 +17,29 @@
     OMS_SITE_NAME: str = "oms"
     OMS_SITE_ADDRESS: str = OMS_SITE_NAME
     API_SITE_ADDRESS: str = jp(("api", SITE_ADDRESS))
     BITRIX_SITE_URL: str = "bitrix.cmrt.ru"
 
     ZABBIX_SITE_NAME: str = "zabbix"
     ZABBIX_SITE: str = ""
-    ZABBIX_SITE_INTERNAL: str = j((ZABBIX_SITE_NAME, SPLITTER, 8080))
-    ZABBIX_SITE_REMOTE: str = j((jp((ZABBIX_SITE_NAME, SITE_ADDRESS)), SPLITTER, 58080))
+    ZABBIX_SITE_INTERNAL: str = j((ZABBIX_SITE_NAME, CONST.SPLITTER, 8080))
+    ZABBIX_SITE_REMOTE: str = j((jp((ZABBIX_SITE_NAME, SITE_ADDRESS)), CONST.SPLITTER, 58080))
 
 
 class EMAIL_COLLECTION:
     MAIL_RU_NAME: str = "mail.ru"
     MAIL_RU_DAEMON: str = jp(("mailer-daemon@corp", MAIL_RU_NAME))
     MAIL_RU_IMAP_SERVER: str = jp(("imap", MAIL_RU_NAME))
 
-    NAS: str = j(("nas", ADDRESSES.SITE_ADDRESS), EMAIL_SPLITTER)
-    IT: str = j(("it", ADDRESSES.SITE_ADDRESS), EMAIL_SPLITTER)
+    NAS: str = j(("nas", ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER)
+    IT: str = j(("it", ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER)
     RECEPTION: str = j(
-        (ADDRESSES.RECEPTION_NAME, ADDRESSES.SITE_ADDRESS), EMAIL_SPLITTER
+        (ADDRESSES.RECEPTION_NAME, ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER
     )
     ADD_EMAIL: str = j(
-        (ADDRESSES.ADD_EMAIL_NAME, ADDRESSES.SITE_ADDRESS), EMAIL_SPLITTER
+        (ADDRESSES.ADD_EMAIL_NAME, ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER
+    )
+    EXTERNAL: str = js(
+        ("mail.", ADDRESSES.SITE_NAME, CONST.EMAIL_SPLITTER, MAIL_RU_NAME)
     )
-    EXTERNAL: str = js(("mail.", ADDRESSES.SITE_NAME, EMAIL_SPLITTER, MAIL_RU_NAME))
 
     EXTERNAL_SERVER: str = MAIL_RU_IMAP_SERVER
```

### Comparing `pih-0.33/pih/consts/date_time.py` & `pih-0.34/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/errors.py` & `pih-0.34/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/events.py` & `pih-0.34/pih/consts/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,14 +460,21 @@
     POLIBASE_PERSON_WAS_CREATED = EventDescription(
         "Создана полибейс персона: {name} ({pin})",
         LogMessageChannels.POLIBASE,
         LogMessageFlags.NOTIFICATION,
         (PARAM_ITEMS.NAME, PARAM_ITEMS.PIN, PARAM_ITEMS.VALUE),
     )
 
+    POLIBASE_PERSON_ANSWERED = EventDescription(
+        "Пациент: {} ({}) ответил: {} на получение ссылки",
+        LogMessageChannels.POLIBASE,
+        (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE),
+        (PARAM_ITEMS.PIN, PARAM_ITEMS.TELEPHONE_NUMBER, PARAM_ITEMS.VALUE),
+    )
+
     MAIL_TO_POLIBASE_PERSON_WAS_SENT = EventDescription(
         "Почта с медицинской записью {id} была отправлена пациенту: {pin}",
         LogMessageChannels.POLIBASE,
         LogMessageFlags.NOTIFICATION,
         (PARAM_ITEMS.ID, PARAM_ITEMS.PIN),
     )
```

### Comparing `pih-0.33/pih/consts/hosts.py` & `pih-0.34/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/names.py` & `pih-0.34/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/password.py` & `pih-0.34/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/paths.py` & `pih-0.34/pih/consts/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,17 @@
     @staticmethod
     def STORAGE() -> str:
         return os.path.join(r"\\", Hosts.DC1.NAME, PATH_FACADE.SHARED_POINT_PATH)
 
     class DITRIBUTIVE:
 
         DELIMITER: str = "-"
-        FOLDER_NAME: str = "dist"
+        FOLDER_NAME: str = ".distr"
         PACKAGE_FOLDER_NAME: str = "all"
+        DEFAULT_PACKAGE_TAG: str = "py3-none-any"
 
         @staticmethod
         def NAME(value: str, version: str | None = None) -> str:
             return j(
                 (ROOT_MODULE_NAME, value, None if n(version) else j(("==", version))),
                 PATH_FACADE.DITRIBUTIVE.DELIMITER,
             )
@@ -86,15 +87,15 @@
                     bdist_wheel_cmd.ensure_finalized()
                     dist_name = bdist_wheel_cmd.wheel_dist_name
                     tag = PATH_FACADE.DITRIBUTIVE.DELIMITER.join(
                         bdist_wheel_cmd.get_tag()
                     )
                 except BaseException as _:
                     dist_name = PATH_FACADE.DITRIBUTIVE.DELIMITER.join((name, version))
-                    tag = "py3-none-any"
+                    tag = PATH_FACADE.DITRIBUTIVE.DEFAULT_PACKAGE_TAG
                 return PathTool.add_extension(
                     j((dist_name, PATH_FACADE.DITRIBUTIVE.DELIMITER, tag)),
                     PYTHON.PACKAGE_EXTENSION,
                 )
 
             return os.path.join(
                 *[
@@ -108,15 +109,15 @@
 
     class VIRTUAL_ENVIRONMENT:
 
         NAME_PREFIX: str = ".venv"
 
 
 class PATH_DATA_STORAGE:
-    NAME: str = "data"
+    NAME: str = ".data"
     VALUE: str = os.path.join(PATH_FACADE.VALUE, NAME)
 
 
 class PATH_BUILD:
     NAME: str = "build"
     VALUE: str = os.path.join(PATH_FACADE.VALUE, NAME)
```

### Comparing `pih-0.33/pih/consts/polibase.py` & `pih-0.34/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/service.py` & `pih-0.34/pih/consts/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,8 +25,12 @@
     @host.setter
     def host(self, value: str | Hosts | Host) -> None:
         if isinstance(value, str):
             self.value.host = value
         elif isinstance(value, Hosts):
             self.host = value.value
         elif isinstance(value, Host):
-            self.host = value.name
+            self.host = value.name
+            
+    @property
+    def NAME(self) -> str | None:
+        return self.value.name
```

### Comparing `pih-0.33/pih/consts/service_commands.py` & `pih-0.34/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/service_roles.py` & `pih-0.34/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/consts/settings.py` & `pih-0.34/pih/consts/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,25 +104,22 @@
 
     TIME_TRACKING_FOR_POLYCLINIC = StringListStorageVariableHolder(
         "TIME_TRACKING_FOR_POLYCLINIC",
         (
             "190",
             "035",
             "058",
-            "064",
             "101-0-",
             "125",
             "131",
-            "134",
             "139",
-            "156",
             "177",
-            "199",
             "124",
             "183",
+            "045"
         ),
     )
 
     POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME = TimeStorageVariableHolder(
         "POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME", "23:00"
     )
     #
```

### Comparing `pih-0.33/pih/pih.py` & `pih-0.34/pih/pih.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-import ipih
-import calendar
-from collections import defaultdict
-from concurrent import futures
+from argparse import ArgumentParser, Namespace, ArgumentError
+from subprocess import DEVNULL, STDOUT, CompletedProcess
+from contextlib import contextmanager, redirect_stdout
+from pkg_resources import parse_version, working_set
+from urllib.parse import unquote, quote_plus, quote
 from concurrent.futures import ThreadPoolExecutor
+from requests import ConnectTimeout, Response
+from colorama import Back, Style, Fore, ansi
+from typing import Any, Callable, TypeAlias
 from datetime import datetime, timedelta
-from getpass import getpass
+from collections import defaultdict
+from prettytable import PrettyTable
+from colorama.ansi import CSI, OSC
+from transliterate import translit
+from concurrent import futures
+from random import randrange
 from threading import Thread
-from time import sleep
+from string import Formatter
 from grpc import StatusCode
+from getpass import getpass
+from functools import cache
+from io import StringIO
+from json import dumps
+from time import sleep
 import importlib.util
+from enum import Enum
 import dataclasses
-import platform
-import locale
-import json
-import re
-import os
-import pathlib
 import subprocess
-from subprocess import DEVNULL, STDOUT, CompletedProcess
-import sys
-from typing import Any, Callable
+import traceback
+import platform
+import calendar
 import colorama
-from colorama import Back, Style, Fore, ansi
-from colorama.ansi import CSI, OSC
-from prettytable import PrettyTable
 import requests
-from requests import ConnectTimeout, Response
-import traceback
+import pathlib
+import locale
 import base64
+import json
 import uuid
-from enum import Enum
-from string import Formatter
-from argparse import ArgumentParser, Namespace, ArgumentError
-from io import StringIO
-from contextlib import contextmanager, redirect_stdout
-from urllib.parse import unquote, quote_plus, quote
-from transliterate import translit
-from functools import cache
-from pkg_resources import parse_version, working_set
+import sys
+import re
+import os
 
-####################################
+import ipih
+from pih.rpc import *
+from pih.tools import *
 from pih.consts import *
 from pih.collections import *
 from pih.consts.errors import *
 from pih.consts.polibase import *
 from pih.consts.python import PYTHON
 from pih.consts.events import Events
+from pih.consts.zabbix import ZABBIX
 from pih.consts.settings import SETTINGS
 from pih.consts.ssh_hosts import SSHHosts
-from pih.consts.zabbix import ZABBIX
 from pih.consts.rpc import RPC as CONST_RPC
 from pih.consts.addresses import ADDRESSES, EMAIL_COLLECTION
-from pih.tools import *
-from pih.consts.service import SUPPORT_NAME_PREFIX, EVENT_LISTENER_NAME_PREFIX
 from pih.tools.service import ServiceRoleTool, ServiceTool, ServiceAdminTool
-from pih.rpc import *
-from random import randrange
-from json import dumps
+from pih.consts.service import SUPPORT_NAME_PREFIX, EVENT_LISTENER_NAME_PREFIX
+
+strdict: TypeAlias = dict[str, Any]
 
 
 class PIHThreadPoolExecutor(ThreadPoolExecutor):
 
     wrapper: Callable
 
     def submit(self, fn, /, *args, **kwargs):
@@ -378,15 +379,15 @@
     def make_separated_lines(self):
         yield True
 
     def write_result(
         self,
         result: Result[T],
         use_index: bool = True,
-        item_separator: str = "\n",
+        item_separator: str = nl(),
         empty_result_text: str = "Не найдено",
         separated_result_item: bool = True,
         label_function: Callable[[Any, int], str] | None = None,
         data_label_function: (
             Callable[[int, FieldItem, Result[T], Any], tuple[bool, str]] | None
         ) = None,
         title: str | None = None,
@@ -937,26 +938,26 @@
     def arg_namespace(self) -> Namespace:
         return self.arg_parser.parse_args()
 
     def named_arg(self, name: str) -> str | None:
         return self.arg_parser.parse_args().__getattribute__(name)
 
     def isolated_arg(self) -> str | None:
-        return self.named_arg(ISOLATED_ARG_NAME)
+        return self.named_arg(CONST.ISOLATED_ARG_NAME)
 
     def add_arg(self, *args, **kwargs) -> bool:
         try:
             self.arg_parser.add_argument(j((ARGUMENT_PREFIX, args[0])), **kwargs)
         except ArgumentError as _:
             return False
         return True
 
     def add_isolated_arg(self) -> bool:
         return self.add_arg(
-            ISOLATED_ARG_NAME,
+            CONST.ISOLATED_ARG_NAME,
             help="Service isolated flag",
             nargs="?",
             const=1,
             type=str,
             default=None,
         )
 
@@ -984,15 +985,15 @@
                 self.output.head1(
                     f"{FullNameTool.to_given_name(PIH.RESULT.USER.by_login(login, cached=False).data.name)}, пожалуйста, пройдите аутентификацию..."
                 )
                 self.output.new_line()
                 if not self.input.yes_no(f"Использовать логин '{login}'", True):
                     login = PIH.input.login()
                 password: str = PIH.input.password(is_new=False)
-                if DataTool.rpc_unrepresent(
+                if DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.authenticate, (login, password)
                     )
                 ):
                     self.authenticated = True
                     self.start(login, False)
                     PIH.EVENT.login()
@@ -1303,15 +1304,15 @@
             self.locked = False
             thread = None
 
     def write_result(
         self,
         result: Result[T],
         use_index: bool = True,
-        item_separator: str = "\n",
+        item_separator: str = nl(),
         empty_result_text: str = "Не найдено",
         separated_result_item: bool = True,
         label_function: Callable[[Any, int], str | list[str]] | None = None,
         data_label_function: (
             Callable[[int, FieldItem, T, Any], tuple[bool, str]] | None
         ) = None,
         title: str | None = None,
@@ -1836,15 +1837,18 @@
                 )
                 if e(selected_index):
                     if use_free_input:
                         return value
                     selected_index = -1
                 try:
                     selected_index = int(selected_index) - min_value
-                    if selected_index >= 0 and selected_index < length:
+                    if (
+                        selected_index >= 0
+                        and selected_index < length + zero_index_value
+                    ):
                         return selected_index
                 except ValueError:
                     has_error = True
                     continue
 
     def item_by_index(
         self,
@@ -2060,15 +2064,15 @@
             result = result.replace(minute=0, hour=0)
         return result
 
     def choose_file(
         self, use_search_request: bool | None = None, allow_choose_all: bool = False
     ) -> File | list[File]:
         if n(use_search_request):
-            use_search_request = self.yes_no("Использвать поиск")
+            use_search_request = self.yes_no("Использовать поиск")
         file_list: list[File] | None = None
         search_request: str = self.input("Введите поисковый запрос")
         with self.output.make_loading(1, "Идет загрузка файлов. Ожидайте"):
             file_list = PIH.RESULT.FILES.find(
                 value=(search_request if use_search_request else None)
             ).data
         if e(file_list):
@@ -2080,27 +2084,27 @@
                         "не найден",
                     )
                 )
             )
             file_list = PIH.RESULT.FILES.all().data
 
         def label_function(file: File, _) -> str:
-            title_list: list[str] = file.title.split(SPLITTER)
+            title_list: list[str] = file.title.split(CONST.SPLITTER)
             if len(title_list) == 3:
                 return j(
                     (
-                        PIH.output.bold(title_list[0].upper()),
+                        self.output.bold(title_list[0].upper()),
                         ": ",
                         title_list[-1],
                         " (",
                         title_list[-2],
                         ")",
                     )
                 )
-            return PIH.output.bold(title_list[1])
+            return self.output.bold(title_list[1])
 
         return self.item_by_index(
             "Выберите файл",
             file_list,  # type: ignore
             label_function,
             allow_choose_all=allow_choose_all,
         )
@@ -2125,15 +2129,15 @@
                             "не найден",
                         )
                     )
                 )
                 note_list = PIH.RESULT.NOTES.all().data
 
             def label_function(note: Note, _) -> str:
-                return PIH.output.bold(note.title)
+                return self.output.bold(note.title)
 
             return self.item_by_index(
                 "Выберите файл",
                 note_list,
                 label_function,
                 allow_choose_all=allow_choose_all,
             )
@@ -2332,34 +2336,34 @@
             FIELD_COLLECTION.AD.SEARCH_ATTRIBUTE,
         )
 
     def search_value(self, search_attribute: str) -> str:
         field_item = FIELD_COLLECTION.AD.SEARCH_ATTRIBUTE.get_item_by_name(
             search_attribute
         )
-        return self.parent.input(f"Введите {field_item.caption.lower()}")
+        return self.parent.input(js(("Введите", lw(field_item.caption))))
 
     def generate_password(
         self, once: bool = False, settings: PasswordSettings = PASSWORD.SETTINGS.DEFAULT
     ) -> str:
-        def internal_generate_password(settings: PasswordSettings = None) -> str:
+        def internal_generate_password(settings: PasswordSettings | None = None) -> str:
             return PasswordTools.generate_random_password(
                 settings.length,
                 settings.special_characters,
                 settings.order_list,
                 settings.special_characters_count,
                 settings.alphabets_lowercase_count,
                 settings.alphabets_uppercase_count,
                 settings.digits_count,
                 settings.shuffled,
             )
 
         while True:
             password = internal_generate_password(settings)
-            if once or self.parent.yes_no(f"Использовать пароль {password}", True):
+            if once or self.parent.yes_no(js(("Использовать пароль", password)), True):
                 return password
             else:
                 pass
 
     def generate_login(
         self,
         full_name: FullName,
@@ -2550,15 +2554,15 @@
             # return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.value < PIH.VERSION.remote()
 
     class INPUT_WAIT:
         NAME: str = "RecipientWaitingForInput"
 
         @staticmethod
         def _get_name(group_name: str, recipient: str) -> str:
-            return j((group_name, recipient), SPLITTER)
+            return j((group_name, recipient), CONST.SPLITTER)
 
         @staticmethod
         def add(group_name: str, recipient: str, timeout: int) -> bool:
             return PIH.ACTION.DATA_STORAGE.value(
                 RecipientWaitingForInput(
                     group_name, timeout, recipient, PIH.DATA.now()
                 ),
@@ -3478,30 +3482,34 @@
                     + if_else(e(login), [], lambda: ["-u", login])
                     + if_else(e(password), [], lambda: ["-p", password])
                 )
                 + command
             )
 
         @staticmethod
-        def create_command_for_powershell(
-            command: list[str],
+        def create_command_for_powershell(command: tuple[str, ...]) -> tuple[str, ...]:
+            if command[0].lower() != CONST.POWERSHELL.NAME:
+                command = (CONST.POWERSHELL.NAME,) + command
+            return command
+
+        @staticmethod
+        def create_command_for_psexec_powershell(
+            command: tuple[str, ...],
             host: str | None = None,
             login: str | None = None,
             password: str | None = None,
             interactive: bool | None = False,
             run_from_system_account: bool = False,
             run_with_elevetion: bool = False,
             allow_use_local_host: bool = True,
             use_raw_host_name: bool = False,
             use_raw_login: bool = False,
-        ) -> list[str]:
-            if command[0].lower() != CONST.POWERSHELL.NAME:
-                command.insert(0, CONST.POWERSHELL.NAME)
+        ) -> tuple[str, ...]:
             return PIH.EXECUTOR.create_command_for_psexec(
-                command,
+                PIH.EXECUTOR.create_command_for_powershell(command),
                 host,
                 login,
                 password,
                 interactive,
                 run_from_system_account,
                 run_with_elevetion,
                 allow_use_local_host,
@@ -3704,20 +3712,20 @@
                 if PIH.DATA.CHECK.returncode(result):
                     return result
             return None
 
         @staticmethod
         def execute_python_localy(
             text: str,
-            parameters: dict[str, Any] | None = None,
+            parameters: strdict | None = None,
             stdout_redirect: bool | None = True,
             catch_exceptions: bool = False,
             use_default_stdout: bool = False,
-        ) -> str | dict[str, Any] | None:
-            result_parameters: dict[str, Any] = globals()
+        ) -> str | strdict | None:
+            result_parameters: strdict = globals()
             if nn(parameters):
                 for key, value in parameters.items():
                     result_parameters[key] = value
             if "self" not in result_parameters:
                 result_parameters["self"] = OutputStub()
             if "self" in result_parameters:
                 if use_default_stdout:
@@ -3807,15 +3815,15 @@
             host: str | None = None,
             login: str | None = None,
             password: str | None = None,
         ) -> str:
             command_list: list[str] = [
                 "tasklist",
                 "/fi",
-                f"pid eq {pid}",
+                js(("pid", "eq", pid)),
                 "/fo",
                 "list",
             ]
             login = PIH.DATA.FORMAT.login(
                 login
                 or PIH.DATA.VARIABLE.ENVIRONMENT.value(LINK.ADMINISTRATOR_LOGIN, False)
                 or AD.ADMINISTRATOR_LOGIN
@@ -3925,17 +3933,17 @@
 
         @staticmethod
         def server_was_started(name: str) -> None:
             PIH.EVENT.send(Events.SERVER_WAS_STARTED, (name,))
 
         @staticmethod
         def get_parameter(
-            event: Events, parameters: dict[str, Any], parameter_name: str | None = None
-        ) -> Any | dict[str, Any]:
-            parameters_map: dict[str, Any] = PIH.EVENT.BUILDER.create_parameters_map(
+            event: Events, parameters: strdict, parameter_name: str | None = None
+        ) -> Any | strdict:
+            parameters_map: strdict = PIH.EVENT.BUILDER.create_parameters_map(
                 event, parameters
             )
             return DataTool.check_not_none(
                 parameter_name, lambda: parameters_map[parameter_name], parameters_map
             )
 
         class BUILDER:
@@ -3952,15 +3960,15 @@
                 parameters = parameters or ()
                 if check_for_parameters_count and len(parameter_pattern_list) > len(
                     parameters
                 ):
                     raise Exception(
                         "Income parameter list length is less that parameter list length of command"
                     )
-                result: dict[str, Any] = {}
+                result: strdict = {}
                 for index, parameter_pattern_item in enumerate(parameter_pattern_list):
                     if index < len(parameters):
                         parameter_pattern: ParamItem = parameter_pattern_item
                         value: Any = parameters[index]
                         if nn(value):
                             result[parameter_pattern.name] = value
                     else:
@@ -4344,14 +4352,25 @@
                         "Предзапись"
                         if value.pin == POLIBASE.PRERECORDING_PIN
                         else value.pin
                     ),
                     value,
                 ),
             )
+            
+        @staticmethod
+        def polibase_person_answered(who: PolibasePerson, answer: str) -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_PERSON_ANSWERED,
+                (
+                    who.pin,
+                    who.telephoneNumber,
+                    answer,
+                ),
+            )
 
         @staticmethod
         def resource_accessible(resource: ResourceStatus, at_first_time: bool) -> None:
             PIH.EVENT.send(
                 Events.RESOURCE_ACCESSABLE, (resource.name, resource, at_first_time)
             )
 
@@ -4423,15 +4442,15 @@
         def new_polibase_scanned_document_processed(file_path: str) -> None:
             event_ds: EventDS | None = one(
                 PIH.RESULT.EVENTS.get(
                     Events.NEW_POLIBASE_DOCUMENT_DETECTED, (None, file_path)
                 )
             )
             if nn(event_ds):
-                parameters: dict[str, Any] = event_ds.parameters
+                parameters: strdict = event_ds.parameters
                 PIH.EVENT.send(
                     Events.NEW_POLIBASE_DOCUMENT_DETECTED,
                     (
                         parameters[PARAM_ITEMS.PERSON_PIN.name],
                         file_path,
                         parameters[PARAM_ITEMS.DOCUMENT_NAME.name],
                         1,
@@ -4448,16 +4467,16 @@
             login: str = PIH.session.get_login()
             user: User = PIH.RESULT.USER.by_login(login).data
             PIH.EVENT.send(
                 Events.SESSION_STARTED,
                 (
                     user.name,
                     login,
-                    f"{PIH.session.file_name} {argv_str}",
-                    f"{PIH.VERSION.value}",
+                    js((PIH.session.file_name, argv_str)),
+                    PIH.VERSION.value,
                     PIH.SYS.host(),
                 ),
             )
 
         @staticmethod
         def backup_robocopy_job_was_started(
             name: str, job_status: RobocopyJobStatus
@@ -4471,15 +4490,15 @@
             name: str, job_status: RobocopyJobStatus
         ) -> None:
             status: int = job_status.last_status
             is_live: bool = job_status.pid > 0
             status_string: str = "live job" if is_live else str(status)
             pid_string: str = str(job_status.pid) if is_live else "not live job"
             if status >= ROBOCOPY.ERROR_CODE_START:
-                status_string += " (есть ошибки)"
+                status_string = js((status_string, "(есть ошибки)"))
             PIH.EVENT.send(
                 Events.BACKUP_ROBOCOPY_JOB_WAS_COMPLETED,
                 (name, status_string, status, pid_string),
             )
 
         @staticmethod
         def service_is_inaccessable_and_will_be_restarted(
@@ -4641,17 +4660,23 @@
         ) -> None:
             event: Events = Events.POLIBASE_CREATION_DB_DUMP_START
             PIH.EVENT.send(
                 event, flags=None if save else PIH.DATA.EVENT.remove_save_flag(event)
             )
 
         @staticmethod
-        def backup_notify_about_polibase_creation_db_dumb_complete(size: int, save: bool = True) -> None:
+        def backup_notify_about_polibase_creation_db_dumb_complete(
+            size: int, save: bool = True
+        ) -> None:
             event: Events = Events.POLIBASE_CREATION_DB_DUMP_COMPLETE
-            PIH.EVENT.send(Events.POLIBASE_CREATION_DB_DUMP_COMPLETE, (size,), None if save else PIH.DATA.EVENT.remove_save_flag(event))
+            PIH.EVENT.send(
+                Events.POLIBASE_CREATION_DB_DUMP_COMPLETE,
+                (size,),
+                None if save else PIH.DATA.EVENT.remove_save_flag(event),
+            )
 
         @staticmethod
         def backup_notify_about_polibase_creation_archived_db_dumb_start() -> None:
             PIH.EVENT.send(Events.POLIBASE_CREATION_ARCHIVED_DB_DUMP_START)
 
         @staticmethod
         def backup_notify_about_polibase_creation_archived_db_dumb_complete(
@@ -4977,15 +5002,15 @@
             ) -> ServiceDescription:
                 service_description: ServiceDescription = EnumTool.get(
                     ServiceRoles.DEVELOPER
                 )
                 if n(port) or port == service_description.port:
                     return service_description
                 return ServiceDescription(
-                    j(("Developer", port), SPLITTER),
+                    j(("Developer", port), CONST.SPLITTER),
                     host=CONST.HOST.DEVELOPER.NAME,
                     port=CONST_RPC.PORT(port),
                 )
 
             @staticmethod
             def create_support_service_or_master_service_description(
                 master_service_desctiption: ServiceDescription, host: str | None = None
@@ -5000,15 +5025,15 @@
                                             (
                                                 SUPPORT_NAME_PREFIX,
                                                 master_service_desctiption.name,
                                             )
                                         ),
                                         host,
                                     ),
-                                    SPLITTER,
+                                    CONST.SPLITTER,
                                 ),
                                 description=js(
                                     (
                                         "Support service for",
                                         master_service_desctiption.name,
                                         "on",
                                         host,
@@ -5030,15 +5055,15 @@
             @staticmethod
             def create_event_listener_service_description(
                 host: str, port: int
             ) -> ServiceDescription:
                 return ServiceDescription(
                     name=j(
                         (EVENT_LISTENER_NAME_PREFIX, host, port),
-                        SPLITTER,
+                        CONST.SPLITTER,
                     ),
                     description="Subscriber",
                     host=host,
                     port=port,
                     auto_start=False,
                     auto_restart=False,
                 )
@@ -5205,15 +5230,15 @@
                                     host_is_linux=host_is_linux,
                                 )
                             else:
                                 file_path = PIH.PATH.join(
                                     service_description.service_path, service_file  # type: ignore
                                 )
                         command_list.append(file_path)
-                        command_list.append(j((ARGUMENT_PREFIX, ISOLATED_ARG_NAME)))
+                        command_list.append(j((CONST.ARGUMENT_PREFIX, CONST.ISOLATED_ARG_NAME)))
                         command_list.append("0")
                         if ne(parameters):
                             if isinstance(parameters, (list, tuple)):
                                 for parameter_item in parameters:
                                     command_list.append(parameter_item)
                             elif isinstance(parameters, dict):
                                 for parameter_item in parameters:
@@ -5455,15 +5480,15 @@
                 return [], []
 
             @staticmethod
             def request_for_service_information_list() -> None:
                 PIH.SERVICE.ADMIN.update_service_information(
                     DataTool.map(
                         PIH.DATA.EXTRACT.service_information,
-                        DataTool.rpc_unrepresent(
+                        DataTool.rpc_decode(
                             PIH.SERVICE.call_command(
                                 ServiceCommands.get_service_information_list,
                                 ((RPC.service_information or STUB).name),
                             )
                         )
                         or [],
                     ),
@@ -6116,15 +6141,15 @@
 
             @staticmethod
             def get(
                 name: str | None = None, section: Sections | str | None = None
             ) -> StorageVariableHolder | list[StorageVariableHolder] | None:
                 section = section or PIH.DATA.VARIABLE.Sections.VARIABLE
                 section_name: str | None = EnumTool.get(section)
-                data: dict[str, Any] | list[dict[str, Any]] | None = (
+                data: strdict | list[strdict] | None = (
                     PIH.RESULT.DATA_STORAGE.value(
                         name,
                         None if n(name) else StorageVariableHolder,
                         section_name,
                     ).data
                 )
 
@@ -6429,15 +6454,15 @@
                     )
                 )
 
             @staticmethod
             def command_type(value: str | File) -> CommandTypes | None:
                 if isinstance(value, File):
                     return PIH.DATA.EXTRACT.command_type(value.title)
-                value = value.split(SPLITTER)[0]
+                value = value.split(CONST.SPLITTER)[0]
                 for item in CommandTypes:
                     if value.lower() in DataTool.map(
                         lambda item: item.lower(), EnumTool.get(item)[1:]
                     ):
                         return item
                 return None
 
@@ -6559,15 +6584,15 @@
                                 WhatsAppMessage(), parameters[0]
                             )
                             if ne(message.message):
                                 message.message = unquote(message.message)
                     return message
 
                 @staticmethod
-                def action(value: dict[str, Any]) -> ActionWasDone:
+                def action(value: strdict) -> ActionWasDone:
                     action: ActionWasDone = DataTool.fill_data_from_source(
                         ActionWasDone(),
                         PIH.EVENT.get_parameter(Events.ACTION_WAS_DONE, value),
                         copy_by_index=True,
                     )
                     action.action = EnumTool.get(Actions, action.action)
                     return action
@@ -6587,15 +6612,15 @@
                 ) -> tuple[Events, list[Any]]:
                     event_data: Any | list[Any] = (
                         value.values[0]
                         if PIH.DATA.CHECK.has_subscribtion_result(value)
                         else value.values
                     )
                     event: Events = EnumTool.get(Events, event_data[0])
-                    parameters: dict[str, Any] = event_data[1]
+                    parameters: strdict = event_data[1]
                     result_parameters: list[Any] = []
                     if ne(event.value.params):
                         for event_parameters_description in event.value.params:
                             event_parameters_description: ParamItem = (
                                 event_parameters_description
                             )
                             if event_parameters_description.optional:
@@ -6625,15 +6650,15 @@
             ) -> SubscribtionResult | None:
                 def extract() -> SubscriberInformation:
                     result: SubscribtionResult = DataTool.fill_data_from_source(
                         SubscribtionResult(), pl.values[-1]
                     )
                     if isinstance(result.result, str):
                         try:
-                            result.result = DataTool.rpc_unrepresent(result.result)
+                            result.result = DataTool.rpc_decode(result.result)
                         except Exception as _:
                             pass
                     return result
 
                 return (
                     None
                     if e(pl.values) or not PIH.DATA.CHECK.has_subscribtion_result(pl)
@@ -7070,32 +7095,32 @@
                                 )  # type: ignore
                             ),
                         )
                     )  # type: ignore
                 )
 
             class BACKUP:
-                SPLITTER: str = "::"
+                CONST.SPLITTER: str = "::"
 
                 @staticmethod
                 def job_full_name(name: str, source: str, destination: str) -> str:
                     return j(
-                        (source, destination, name), PIH.DATA.FORMAT.BACKUP.SPLITTER
+                        (source, destination, name), PIH.DATA.FORMAT.BACKUP.CONST.SPLITTER
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
-                        PIH.DATA.FORMAT.BACKUP.SPLITTER,
+                        PIH.DATA.FORMAT.BACKUP.CONST.SPLITTER,
                     )
 
             @staticmethod
             def donain(value: str) -> str:
                 return if_else(
                     value.endswith(AD.DOMAIN_DNS),
                     value,
@@ -7142,15 +7167,15 @@
                 return j(
                     (
                         "Остаток по времени (дней):",
                         f" {CONST.VISUAL.BULLET} Максимально: {count * to_days(statistics.max)}",
                         f" {CONST.VISUAL.BULLET} Минимально: {count * to_days(statistics.min)}",
                         f" {CONST.VISUAL.BULLET} В среднем: {count * to_days(statistics.avg)}",
                     ),
-                    "\n",
+                    nl(),
                 )
 
             @staticmethod
             def yes_no(value: bool, symbolic: bool = False) -> str:
                 c: Callable[
                     [
                         bool,
@@ -7180,18 +7205,18 @@
                         "Мб" if use_megabites else "Гб",
                     )
                 )
 
             @staticmethod
             def format(
                 value: str,
-                parameters: dict[str, Any] | None = None,
+                parameters: strdict | None = None,
                 use_python: bool = False,
             ) -> str:
-                result_parameters: dict[str, Any] = globals()
+                result_parameters: strdict = globals()
                 # result_parameters["print"] = print
                 if nn(parameters):
                     for lkey, lvalue in parameters.items():
                         result_parameters[lkey] = lvalue
                 io: StringIO = StringIO()
                 part: str
                 for part in re.findall(
@@ -7229,15 +7254,15 @@
 
             @staticmethod
             def index(value: int) -> str:
                 return str(value + 1) if value > 0 else ""
 
             @staticmethod
             def user_principal_name(login: str) -> str:
-                return j((login, AD.DOMAIN_MAIN), EMAIL_SPLITTER)
+                return j((login, AD.DOMAIN_MAIN), A.CT.EMAIL_SPLITTER)
 
             @staticmethod
             def as_string(
                 value: Any,
                 escaped_string: bool = False,
                 mapper: Callable[[Any], str] | None = None,
             ) -> str | None:
@@ -7246,15 +7271,15 @@
                     result = value.name
                 else:
                     result = str(value)
                 if escaped_string:
                     if isinstance(value, (str, datetime, Enum)):
                         result = escs(result)
                     if isinstance(value, dict):
-                        result = escs(DataTool.rpc_represent(value, False))
+                        result = escs(DataTool.rpc_encode(value, False))
                 return DataTool.check_not_none(mapper, lambda: mapper(result), result)
 
             @staticmethod
             def host(
                 value: str | None,
                 reverse: bool = False,
                 use_default_domain: bool = True,
@@ -7262,19 +7287,19 @@
                 if n(value):
                     return None
                 value = value.lower()
                 host_start: str = r"\\"
                 if reverse:
                     return ListTool.not_empty_items(
                         j(
-                            j(value.replace("\\", SPLITTER)).replace("/", SPLITTER)
-                        ).split(SPLITTER)
+                            j(value.replace("\\", CONST.SPLITTER)).replace("/", CONST.SPLITTER)
+                        ).split(CONST.SPLITTER)
                     )[0]
                 if use_default_domain and not value.endswith(AD.DOMAIN_MAIN):
-                    value = j((value, AD.DOMAIN_MAIN), AD.SPLITTER)
+                    value = j((value, AD.DOMAIN_MAIN), AD.CONST.SPLITTER)
                 return ("" if value.startswith(host_start) else host_start) + value
 
             @staticmethod
             def host_name(value: str) -> str:
                 return value.split(".")[0]
 
             @staticmethod
@@ -7445,29 +7470,29 @@
 
             @staticmethod
             def email(
                 value: str,
                 use_default_domain: bool = False,
                 email_correction: bool = False,
             ) -> str:
-                if use_default_domain and value.find(EMAIL_SPLITTER) == -1:
+                if use_default_domain and value.find(A.CT.EMAIL_SPLITTER) == -1:
                     value = PIH.DATA.FORMAT.email(
-                        j((value, ADDRESSES.SITE_ADDRESS), EMAIL_SPLITTER)
+                        j((value, ADDRESSES.SITE_ADDRESS), A.CT.EMAIL_SPLITTER)
                     )
                 if email_correction:
                     for char in '"(),:;<>[\\] ':
                         value = value.replace(char, "")
                     value = value.replace("/", ".")
-                    email_name, email_domain = value.split(EMAIL_SPLITTER)
+                    email_name, email_domain = value.split(A.CT.EMAIL_SPLITTER)
                     PIH.RESULT.FILES.execute("@email_correction")
                     for email_correction_item in EMAIL_CORRECTION:
                         if email_domain in email_correction_item[0]:
                             email_domain = email_correction_item[1]
                             break
-                    value = j((email_name, email_domain), EMAIL_SPLITTER)
+                    value = j((email_name, email_domain), A.CT.EMAIL_SPLITTER)
                 return value.lower()
 
             @staticmethod
             def name(
                 value: str,
                 remove_non_alpha: bool = False,
                 name_part_minimal_length: int | None = None,
@@ -8010,15 +8035,15 @@
                 return ResultTool.map(
                     convert,
                     PIH.RESULT.EVENTS.get(Events.ADD_JOURNAL_RECORD, parameters),
                 )
 
         class EMAIL:
             @staticmethod
-            def information(value: str) -> Result[dict[str, Any]]:
+            def information(value: str) -> Result[strdict]:
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(
                         ServiceCommands.get_email_information,
                         (value, EmailVerificationMethods.ABSTRACT_API),
                     )
                 )
 
@@ -8053,15 +8078,15 @@
                 count_as_result: bool = False,
             ) -> Result[list[EventDS] | int]:
                 def extract_function(data: Any, count_as_result: bool) -> EventDS | int:
                     if count_as_result:
                         return data
                     result: EventDS = DataTool.fill_data_from_source(EventDS(), data)
                     # from json string to python object
-                    result.parameters = DataTool.rpc_unrepresent(result.parameters)
+                    result.parameters = DataTool.rpc_decode(result.parameters)
                     if isinstance(result.timestamp, str):
                         result.timestamp = DateTimeTool.datetime_from_string(
                             result.timestamp
                         )
                     return result
 
                 return DataTool.to_result(
@@ -8268,15 +8293,15 @@
                         item[0](label)
                     if value in item[1][label][1]:
                         return item[1][label][1][value]
                 return None
 
             @staticmethod
             def _convert_from_event(value: EventDS) -> Result[Note | File]:
-                parameters: dict[str, Any] = value.parameters
+                parameters: strdict = value.parameters
                 result: File | Note | None = File(
                     PIH.DATA.FORMAT.from_mysql(parameters[FIELD_NAME_COLLECTION.TITLE]),
                     PIH.DATA.FORMAT.from_mysql(parameters[FIELD_NAME_COLLECTION.TEXT]),
                     parameters[FIELD_NAME_COLLECTION.ID],
                 )
                 if value.name == Events.SAVE_NOTE_FROM_KNOWLEDGE_BASE.name:
                     result = DataTool.fill_data_from_source(
@@ -8374,51 +8399,51 @@
                         lambda item: PIH.DATA.EXTRACT.command_type(item)
                         == command_type,
                         result,
                     )
                 )
                 result = (
                     ResultTool.filter(
-                        lambda item: item.title.find(j((SPLITTER, "@"))) == -1, result  # type: ignore
+                        lambda item: item.title.find(j((CONST.SPLITTER, "@"))) == -1, result  # type: ignore
                     )
                     if exclude_private_files
                     else result
                 )
 
                 def sort_function(value: File) -> str:
-                    title_list: list[str] = lw(value.title).split(SPLITTER)
+                    title_list: list[str] = lw(value.title).split(CONST.SPLITTER)
                     return j(
-                        [title_list[0]] + [title_list[-1]] + title_list[1:-1], SPLITTER
+                        [title_list[0]] + [title_list[-1]] + title_list[1:-1], CONST.SPLITTER
                     )
 
                 return ResultTool.sort(sort_function, result)
 
             @staticmethod
             def execute(
                 file_search_request: str,
-                parameters: dict[str, Any] | None = None,
+                parameters: strdict | None = None,
                 stdout_redirect: bool | None = True,
                 catch_exceptions: bool = False,
                 use_default_stdout: bool = False,
-            ) -> str | dict[str, Any] | None:
+            ) -> str | strdict | None:
                 file: File | None = one(PIH.RESULT.FILES.find(file_search_request))
                 if n(file):
                     return None
                 return PIH.EXECUTOR.execute_python_localy(
                     file.text,  # type: ignore
                     parameters,
                     stdout_redirect,
                     catch_exceptions,
                     use_default_stdout,
                 )
 
             @staticmethod
             def execute_some(
                 file_search_request: str,
-                parameters: dict[str, Any] | None = None,
+                parameters: strdict | None = None,
                 stdout_redirect: bool = True,
                 catch_exceptions: bool = False,
                 use_default_stdout: bool = False,
             ) -> list[str] | None:
                 file: File | None = None
                 result: list[str] = []
                 file_list: list[File] = PIH.RESULT.FILES.find(file_search_request).data  # type: ignore
@@ -8555,15 +8580,15 @@
             @staticmethod
             def fms_unit_name(code: str) -> Result[str]:
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(ServiceCommands.get_fms_unit_name, (code,))
                 )
 
             @staticmethod
-            def execute(query: str) -> Result[list[dict[str, Any]]]:
+            def execute(query: str) -> Result[list[strdict]]:
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(
                         ServiceCommands.execute_data_source_query, (query,)
                     )
                 )
 
         class MESSAGE:
@@ -8625,15 +8650,15 @@
                     ),
                 )
 
             @staticmethod
             def barcodes_information(
                 file_path: str, get_only_first_barcode: bool = False, log_level: int = 0
             ) -> Result[list[list[BarcodeInformation]]]:
-                def extractor(data: list[dict[str, Any]]) -> list[BarcodeInformation]:
+                def extractor(data: list[strdict]) -> list[BarcodeInformation]:
                     return list(
                         map(
                             lambda item: DataTool.fill_data_from_source(
                                 BarcodeInformation(), item
                             ),
                             data,
                         )
@@ -8970,15 +8995,17 @@
             @staticmethod
             def by_name(value: str) -> Result[Workstation]:
                 try:
                     return PIH.RESULT.COMPUTER.by_name(
                         value, PIH.RESULT.WORKSTATION.CONTAINER_DN, Workstation
                     )
                 except NotFound as _:
-                    raise NotFound(f"Рабочая станция с именем {value} не найден")
+                    raise NotFound(
+                        js(("Рабочая станция с именем", escs(value), "не найден"))
+                    )
 
             @staticmethod
             def all() -> Result[list[Workstation]]:
                 return PIH.RESULT.COMPUTER.by_container_dn(
                     PIH.RESULT.WORKSTATION.CONTAINER_DN, Workstation
                 )
 
@@ -9047,15 +9074,15 @@
                 )
                 start_date = DateTimeTool.begin_date(start_date or now)
                 end_date = DateTimeTool.end_date(end_date or now)
 
                 def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str:
                     return DataTool.check_not_none(
                         entity,
-                        lambda: entity.TimeVal.split(DATE_TIME.SPLITTER)[not date],
+                        lambda: entity.TimeVal.split(DATE_TIME.CONST.SPLITTER)[not date],
                     )
 
                 result_data: dict = {}
                 full_name_by_tab_number_map: dict = {}
                 result_data = defaultdict(
                     lambda: defaultdict(lambda: defaultdict(list))
                 )
@@ -9154,20 +9181,20 @@
                                         index + 1
                                     ]
                                     if nn(item.exit_time):
                                         if nn(item_next.enter_time):
                                             duration = int(
                                                 datetime.fromisoformat(
                                                     item.date
-                                                    + DATE_TIME.SPLITTER
+                                                    + DATE_TIME.CONST.SPLITTER
                                                     + item.exit_time
                                                 ).timestamp()
                                                 - datetime.fromisoformat(
                                                     item_next.date
-                                                    + DATE_TIME.SPLITTER
+                                                    + DATE_TIME.CONST.SPLITTER
                                                     + item_next.enter_time
                                                 ).timestamp()
                                             )
                                             # print(full_name, full_name in has_lunch_break)
                                             # duration -= 60*60 if (full_name in has_lunch_break) else 0
                                             item.duration = duration
                                             person.duration += duration
@@ -9349,58 +9376,59 @@
             def temporary_mark_owner_by_tab_number(value: str) -> Result[Mark]:
                 return PIH.RESULT.MARK.temporary_mark_owner(
                     PIH.RESULT.MARK.by_tab_number(value).data
                 )
 
         class POLIBASE:
             @staticmethod
-            def _person_pin(person_or_pin: PolibasePerson | int) -> int:
+            def _person_pin(value: PolibasePerson | int) -> int:
                 return (
-                    person_or_pin.pin
-                    if isinstance(person_or_pin, PolibasePerson)
-                    else person_or_pin
+                    value.pin
+                    if isinstance(value, PolibasePerson)
+                    else value
                 )
 
             @staticmethod
             def bonus_information(
-                person_or_person_pin: PolibasePerson | int, test: bool | None = None
+                who: PolibasePerson | int, test: bool | None = None
             ) -> Result[BonusInformation]:
                 result: BonusInformation = BonusInformation()
 
                 class DH:
                     last_item: dict[str, int | float] | None = None
 
                 def action(item: dict[str, int | float]) -> None:
                     item["bonus_plus"] = item["bonus_plus"] or 0
                     item["bonus_minus"] = item["bonus_minus"] or 0
                     item["money"] = item["money"] or 0
-                    result.all += item["bonus_plus"]
-                    result.spent += item["bonus_minus"]
+                    result.money_all += item["money"]
+                    result.bonus_all += item["bonus_plus"]
+                    result.bonus_spent_all += item["bonus_minus"]
                     if n(DH.last_item):
                         DH.last_item = item
 
                 ResultTool.every(
                     action,
                     DataTool.to_result(
                         PIH.SERVICE.call_command(
                             ServiceCommands.get_bonus_list,
                             (
-                                PIH.RESULT.POLIBASE._person_pin(person_or_person_pin),
+                                PIH.RESULT.POLIBASE._person_pin(who),
                                 test,
                             ),
                         )
                     ),
                 )
                 if nn(DH.last_item):
-                    result.last_spent = DH.last_item["bonus_minus"]
-                    result.last = (
+                    result.bonus_last_spent = DH.last_item["bonus_minus"]
+                    result.bonus_last = (
                         DH.last_item["bonus_plus"] - DH.last_item["bonus_minus"]
                     )
-                    result.last_money_spent = DH.last_item["money"]
-                    result.active = result.all - result.spent
+                    result.money_last = DH.last_item["money"]
+                    result.bonus_active = result.bonus_all - result.bonus_spent_all
                 return Result(None, result)
 
             @staticmethod
             def workstations_by_login(
                 value: str, test: bool | None = None
             ) -> Result[list[Workstation]] | None:
                 if PIH.CHECK.POLIBASE.person_exists_by_login(value):
@@ -9626,15 +9654,15 @@
                         "идентификационным номером", value
                     )
                 return result
 
             @staticmethod
             def execute(
                 query: str, test: bool | None = None
-            ) -> Result[list[dict[str, Any]]]:
+            ) -> Result[list[strdict]]:
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(
                         ServiceCommands.execute_polibase_query, (query, test)
                     ),
                 )
 
             @staticmethod
@@ -10181,15 +10209,15 @@
                 )
 
         class RECOGNIZE:
             @staticmethod
             def document_type_exists(
                 file_path: str, value: DocumentTypes, log_level: int | None = None
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.document_type_exists,
                         (file_path, EnumTool.get(value), log_level),
                     )
                 )
 
             @staticmethod
@@ -10227,15 +10255,15 @@
                 address_or_ip: str,
                 port: int,
                 host: str | None = None,
                 count: int | None = None,
                 check_all: bool = True,
             ) -> bool:
                 return PIH.CHECK.RESOURCE.accessibility_by_ping(
-                    j((address_or_ip, port), SPLITTER), host, count, check_all
+                    j((address_or_ip, port), CONST.SPLITTER), host, count, check_all
                 )
 
             @staticmethod
             def accessibility_by_smb_port(
                 address_or_ip: str,
                 host: str | None = None,
                 count: int | None = None,
@@ -10339,18 +10367,18 @@
                 value: str,
                 cached: bool = True,
                 verification_method: EmailVerificationMethods | None = None,
             ) -> bool:
                 def internal_accessability(
                     value: str, verification_method: EmailVerificationMethods
                 ) -> bool:
-                    domain: str = value.split(EMAIL_SPLITTER)[1]
+                    domain: str = value.split(A.CT.EMAIL_SPLITTER)[1]
                     if domain == "icloud.com":
                         verification_method = EmailVerificationMethods.NORMAL
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.check_email_accessibility,
                             (value, verification_method, cached),
                         )
                     )
 
                 # if not internal_accessability(value, verification_method):
@@ -10495,15 +10523,15 @@
                         == user.samAccountName,
                         PIH.RESULT.USER.by_property(value),
                     )
                 )
 
             @staticmethod
             def exists_by_login(value: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.check_user_exists_by_login, value
                     )
                 )
 
             @staticmethod
             def user(value: User) -> bool:
@@ -10597,15 +10625,15 @@
                             if cached
                             else internal_accessibility(profile)
                         )
 
         class MARK:
             @staticmethod
             def free(tab_number: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.check_mark_free, tab_number
                     )
                 )
 
             @staticmethod
             def exists_by_full_name(full_name: FullName) -> bool:
@@ -10626,15 +10654,15 @@
             @staticmethod
             def accessibility() -> bool:
                 return PIH.CHECK.ACCESS.by_group(AD.Groups.TimeTrackingReport)
 
         class INVENTORY:
             @staticmethod
             def is_report_file(file_path: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.check_inventory_report, file_path
                     )
                 )
 
             @staticmethod
             def accessibility() -> bool:
@@ -10651,15 +10679,15 @@
                     and PIH.CHECK.ACCESS.polibase()
                 )
 
             @staticmethod
             def person_card_registry_folder(value: str) -> bool:
                 return (
                     value in CONST.CARD_REGISTRY.SUITABLE_FOLDER_NAME_SYMBOL
-                ) or DataTool.rpc_unrepresent(
+                ) or DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.check_polibase_person_card_registry_folder_name,
                         value,
                     )
                 )
 
             @staticmethod
@@ -11235,15 +11263,15 @@
                 user_login: str,
                 workstation_name: str,
                 message: str,
                 timeout: int = 60,
                 method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE,
             ) -> bool:
                 if method_type == WorkstationMessageMethodTypes.REMOTE:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.send_message_to_user_or_workstation,
                             (user_login, workstation_name, message, timeout),
                         )
                     )
 
                 def internal_send_by_login_and_workstation_name(
@@ -11320,15 +11348,15 @@
                             Message(message, recipient, sender.value), high_priority
                         )
 
                     @staticmethod
                     def add_message(
                         message: Message, high_priority: bool = False
                     ) -> bool:
-                        return DataTool.rpc_unrepresent(
+                        return DataTool.rpc_decode(
                             PIH.SERVICE.call_command(
                                 ServiceCommands.add_message_to_queue,
                                 (message, high_priority),
                             )
                         )
 
                 WAPPI_PROFILE_MAP: dict | None = None
@@ -11409,18 +11437,18 @@
                             for message_item in response_result[key]:
                                 if message_item["type"] == "chat":
                                     result.append(
                                         WhatsAppMessage(
                                             message_item["body"],
                                             message_item["fromMe"],
                                             str(message_item["from"]).split(
-                                                EMAIL_SPLITTER
+                                                A.CT.EMAIL_SPLITTER
                                             )[0],
                                             str(message_item["to"]).split(
-                                                EMAIL_SPLITTER
+                                                A.CT.EMAIL_SPLITTER
                                             )[0],
                                             profile,
                                             message_item["time"],
                                         )
                                     )
                     return result
 
@@ -11715,24 +11743,24 @@
                         EnumTool.get(CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT),
                     ),
                 )
 
         class DELAYED:
             @staticmethod
             def register(message: DelayedMessage) -> int:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.register_delayed_message,
                         PIH.ACTION.MESSAGE.DELAYED._prepeare_message(message),
                     )
                 )
 
             @staticmethod
             def send(message: DelayedMessage, high_priority: bool = True) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.send_delayed_message,
                         (
                             PIH.ACTION.MESSAGE.DELAYED._prepeare_message(message),
                             high_priority,
                         ),
                     )
@@ -11800,15 +11828,15 @@
                     ),
                     " group by parameters->",
                     escs(j(("$.", folder_field_name))),
                     " order by count;",
                 )
             )
 
-            def map_function(value: dict[str, Any]) -> CardRegistryFolderStatistics:
+            def map_function(value: strdict) -> CardRegistryFolderStatistics:
                 result: CardRegistryFolderStatistics = DataTool.fill_data_from_source(
                     CardRegistryFolderStatistics(), value
                 )
                 result.name = json.loads(result.name)
                 return result
 
             return DataTool.get_first_item(
@@ -11960,15 +11988,15 @@
 
     class ACTION:
 
         class ZABBIX:
 
             @staticmethod
             def send(host: str, key: str, value: Any) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call(
                         ServiceRoles.ZABBIX,
                         ServiceCommands.serve_command,
                         (ZABBIX.Commands.send_value.name, host, key, value),
                     )
                 )
 
@@ -11988,42 +12016,42 @@
 
         class RECOGNIZE:
             @staticmethod
             def recognize_document(
                 file_path: str, document_type: DocumentTypes | None = None
             ) -> bool:
                 document_type = document_type or DocumentTypes.POLIBASE
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.recognize_document,
                         (file_path, EnumTool.get(document_type)),
                     )
                 )
 
         class SSH:
             @staticmethod
             def mount_facade_for_linux_host(value: str | None) -> bool | None:
                 if n(value) and not PIH.SYS.is_linux():
                     return None
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.mount_facade_for_linux_host,
                         (value or PIH.SYS.host(),),
                     )
                 )
 
         class JOURNAL:
             @staticmethod
             def add(
                 applicant_user: User,
                 journal_type: JournalType,
                 tag: Tags,
                 title: str,
                 text: str,
-                parameters: dict[str, Any] | None = None,
+                parameters: strdict | None = None,
             ) -> bool:
                 def escape_string(value: str) -> str:
                     value = value.replace('"', "''")
                     value = value.replace("\\", "\\\\")
                     return value
 
                 journal_type_value: tuple[int, OrderedNameCaptionDescription] = (
@@ -12050,26 +12078,26 @@
             @staticmethod
             def send(recipient: str, subject: str, message: str) -> bool | None:
                 if not PIH.CHECK.email(recipient):
                     recipient = PIH.DATA.FORMAT.email(
                         recipient, use_default_domain=True
                     )
                 if PIH.CHECK.email(recipient, check_accesability=True):
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.send_email,
                             (recipient, j(("Subject:", nl(subject, count=2), message))),
                         )
                     )
                 return None
 
         class PATH:
             @staticmethod
             def listen(value: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.listen_for_new_files, (value,)
                     )
                 )
 
         class ACTIONS:
             @staticmethod
@@ -12115,43 +12143,43 @@
                 )
                 return True
 
         class EVENTS:
             @staticmethod
             def register(
                 value: Events,
-                parameters: dict[str, Any] | tuple[Any, ...] | None = None,
+                parameters: strdict | tuple[Any, ...] | None = None,
                 remove_before: bool = False,
             ) -> bool:
                 if isinstance(parameters, Tuple):
                     parameters = PIH.EVENT.BUILDER.create_parameters_map(
                         value, parameters
                     )
                 event_description: EventDescription = EnumTool.get(value)
                 if remove_before:
-                    parameters_for_removing: dict[str, Any] | None = parameters
+                    parameters_for_removing: strdict | None = parameters
                     key_name_list: tuple[str, ...] | None = DataTool.map(
                         lambda item: item.name,
                         DataTool.filter(
                             lambda item: item.key, event_description.params
                         ),
                     )
                     if nn(key_name_list):
                         parameters_for_removing = {}
                         for key_name_item in key_name_list:
                             parameters_for_removing[key_name_item] = parameters[
                                 key_name_item
                             ]
                     PIH.ACTION.EVENTS.remove(value, parameters_for_removing)
-                visible_parameters: dict[str, Any] = {}
+                visible_parameters: strdict = {}
                 for index, parameter_key in enumerate(parameters):
                     if event_description.params[index].saved:
                         visible_parameters[parameter_key] = parameters[parameter_key]
                 parameters = visible_parameters
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.register_event,
                         (
                             EventDS(
                                 value.name,
                                 parameters,
                                 DateTimeTool.now(use_microsecond=True),
@@ -12180,17 +12208,17 @@
                 return PIH.ACTION.EVENTS.remove(
                     *PIH.EVENT.BUILDER.by_key(event_type, parameters)
                 )
 
             @staticmethod
             def remove(
                 value: Events,
-                parameters: tuple[Any, ...] | dict[str, Any] | None = None,
+                parameters: tuple[Any, ...] | strdict | None = None,
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.remove_event,
                         EventDS(
                             value.name,
                             DataTool.check(
                                 isinstance(parameters, dict),
                                 parameters,
@@ -12259,24 +12287,24 @@
                 name: str,
                 title: str,
                 note: Note,
                 label_list: list[str] | None = None,
                 color: str | None = None,
                 raw: bool = False,
             ) -> bool:
-                id: str | None = DataTool.rpc_unrepresent(
+                id: str | None = DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_note, (note, label_list, color, raw)
                     )
                 )
                 if raw:
                     return True
                 if e(id):
                     return False
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.add_gkeep_item, (name, title, id)
                     )
                 )
 
             @staticmethod
             def create_raw(
@@ -12287,33 +12315,33 @@
                 return PIH.ACTION.NOTES.create(
                     None, None, note, label_list, color, True
                 )
 
             @staticmethod
             def drop_cache(local: bool = False) -> bool:
                 if not local:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(ServiceCommands.drop_note_cache)
                     )
                 return True
 
         class QR_CODE:
             @staticmethod
             def titled(
                 data: str, title, path: str, font_size: int | None = None
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_qr_code, (data, title, path, font_size)
                     )
                 )
 
             @staticmethod
             def print(path: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(ServiceCommands.print_image, (path,))
                 )
 
             @staticmethod
             def for_mobile_helper_command(
                 value: str, title: str, path: str, font_size: int | None = None
             ) -> bool:
@@ -12336,15 +12364,15 @@
                     80,
                 )
 
         class INDICATION:
             class CT:
                 @staticmethod
                 def register(value: CTIndicationsValue, forced: bool = False) -> bool:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.register_ct_indications_value,
                             (value, forced),
                         )
                     )
 
             class CHILLER:
@@ -12400,15 +12428,15 @@
             @staticmethod
             def start_robocopy_job(
                 name: str | None = None,
                 source: str | None = None,
                 destination: str | None = None,
                 force: bool = False,
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.robocopy_start_job,
                         (name, source, destination, force),
                     )
                 )
 
             @staticmethod
@@ -12421,27 +12449,27 @@
                 value: Any, name: str | None = None, section: str | None = None
             ) -> bool:
                 try:
                     name = name or value.__getattribute__("name")
                 except AttributeError as error:
                     pass
                 else:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.set_storage_value, (name, value, section)
                         )
                     )
 
         class MESSAGE:
             class DELAYED:
                 @staticmethod
                 def update(
                     value: DelayedMessageDS, search_critery: MessageSearchCritery
                 ) -> bool:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.update_delayed_message,
                             (value, search_critery),
                         )
                     )
 
                 @staticmethod
@@ -12486,15 +12514,15 @@
                                 CONST.INTERNATIONAL_TELEPHONE_NUMBER_PREFIX,
                             )
                     return message
 
         class SETTINGS:
             @staticmethod
             def key(key: str, value: Any) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_settings_value, (key, value)
                     )
                 )
 
             @staticmethod
             def set(settings_item: SETTINGS | str, value: Any) -> bool:
@@ -12512,29 +12540,29 @@
                 return PIH.ACTION.SETTINGS.set(
                     settings_item, settings_item.value.default_value
                 )
 
         class USER:
             @staticmethod
             def drop_user_cache() -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(ServiceCommands.drop_user_cache)
                 )
 
             @staticmethod
             def create_from_template(
                 container_dn: str,
                 full_name: FullName,
                 login: str,
                 password: str,
                 description: str,
                 telephone: str,
                 email: str,
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_user_by_template,
                         (
                             container_dn,
                             full_name,
                             login,
                             password,
@@ -12543,63 +12571,63 @@
                             email,
                         ),
                     )
                 )
 
             @staticmethod
             def set_telephone_number(user: User, telephone: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_user_telephone_number,
                         (user.distinguishedName, telephone),
                     )
                 )
 
             @staticmethod
             def set_password(user: User, password: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_user_password,
                         (user.distinguishedName, password),
                     )
                 )
 
             @staticmethod
             def set_status(user: User, status: str, container: UserBase) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_user_status,
                         (
                             user.distinguishedName,
                             status,
                             DataTool.check(
                                 container, lambda: container.distinguishedName
                             ),
                         ),
                     )
                 )
 
             @staticmethod
             def remove(user: User) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.remove_user, user.distinguishedName
                     )
                 )
 
         class TIME_TRACKING:
             @staticmethod
             def save_report(
                 path: str,
                 start_date: datetime,
                 end_date: datetime,
                 tab_number_list: list[str] | None = None,
                 plain_format: bool = False,
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.save_time_tracking_report,
                         (
                             path,
                             DateTimeTool.begin_date(start_date),
                             DateTimeTool.end_date(end_date),
                             tab_number_list,
@@ -12607,35 +12635,35 @@
                         ),
                     )
                 )
 
         class INVENTORY:
             @staticmethod
             def create_barcodes(report_file_path: str, result_directory: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_barcodes_for_inventory,
                         (report_file_path, result_directory),
                     )
                 )
 
             @staticmethod
             def save_report_item(
                 report_file_path: str, item: InventoryReportItem
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.save_inventory_report_item,
                         (report_file_path, item),
                     )
                 )
 
             @staticmethod
             def close_report(report_file_path: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.close_inventory_report, report_file_path
                     )
                 )
 
         class PRINTER:
             @staticmethod
@@ -12649,15 +12677,15 @@
         class POLIBASE:
             executor: PIHThreadPoolExecutor = PIHThreadPoolExecutor(max_workers=10)
 
             def update_person_change_date(
                 polibase_person: PolibasePerson,
                 registrator_polibase_person: PolibasePerson,
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.update_person_change_date,
                         (polibase_person.pin, registrator_polibase_person.pin),
                     )
                 )
 
             @staticmethod
@@ -12703,48 +12731,48 @@
                 PIH.EXECUTOR.ws_reboot(
                     Hosts.POLIBASE_TEST.NAME if test else Hosts.POLIBASE.NAME
                 )
 
             class NOTIFICATION:
                 @staticmethod
                 def register(value: PolibasePersonVisitNotificationDS) -> bool:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.register_polibase_person_visit_notification,
                             value,
                         )
                     )
 
                 class CONFIRMATION:
                     @staticmethod
                     def update(recepient: str, sender: str, status: int) -> bool:
-                        return DataTool.rpc_unrepresent(
+                        return DataTool.rpc_decode(
                             PIH.SERVICE.call_command(
                                 ServiceCommands.update_polibase_person_notification_confirmation,
                                 PolibasePersonNotificationConfirmation(
                                     recepient, sender, status
                                 ),
                             )
                         )
 
             class INFORMATION_QUEST:
                 @staticmethod
                 def register(person: PolibasePerson) -> bool:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.register_polibase_person_information_quest,
                             PolibasePersonInformationQuest(
                                 person.pin, person.FullName, person.telephoneNumber
                             ),
                         )
                     )
 
                 @staticmethod
                 def start(person_or_pin: PolibasePerson | int) -> bool:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.start_polibase_person_information_quest,
                             (
                                 (
                                     person_or_pin
                                     if isinstance(person_or_pin, int)
                                     else person_or_pin.pin
@@ -12754,95 +12782,98 @@
                     )
 
                 @staticmethod
                 def update(
                     value: PolibasePersonInformationQuest,
                     search_critery: PolibasePersonInformationQuest,
                 ) -> bool:
-                    return DataTool.rpc_unrepresent(
+                    return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.update_polibase_person_information_quest,
                             (value, search_critery),
                         )
                     )
 
             @staticmethod
             def create_barcode_for_person(
                 person_or_pin: PolibasePerson | int, test: bool | None = None
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_barcode_for_polibase_person,
                         (PIH.RESULT.POLIBASE._person_pin(person_or_pin), test),
                     )
                 )
 
             @staticmethod
             def set_card_registry_folder(
                 value: str | None,
                 person: PolibasePerson,
                 test: bool | None = None,
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_polibase_person_card_folder_name,
                         (value, PIH.RESULT.POLIBASE._person_pin(person), test),
                     )
                 )
 
             @staticmethod
             def email(
                 value: str, person: PolibasePerson, test: bool | None = None
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_polibase_person_email,
                         (value, person.pin, test),
                     )
                 )
 
             @staticmethod
             def set_telephone_number(
                 index: int, value: str, person: PolibasePerson, test: bool | None = None
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_polibase_person_telephone_number,
                         (index, value, person.pin, test),
                     )
                 )
 
             @staticmethod
             def set_barcode(
                 value: str, person: PolibasePerson, test: bool | None = None
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_barcode_for_polibase_person,
                         (value, person.pin, test),
                     )
                 )
 
             class DB:
                 @staticmethod
                 def backup(
                     dump_file_name: str | None = None,
                     test: bool | None = None,
                 ) -> bool:
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_polibase_database_backup,
-                        (dump_file_name, test,),
+                        (
+                            dump_file_name,
+                            test,
+                        ),
                     )
                     return True
 
             class VISIT:
                 class DATA_STORAGE:
                     @staticmethod
                     def update(value: PolibasePersonVisitDS) -> bool:
-                        return DataTool.rpc_unrepresent(
+                        return DataTool.rpc_decode(
                             PIH.SERVICE.call_command(
                                 ServiceCommands.update_polibase_person_visit_to_data_stogare,
                                 value,
                             )
                         )
 
         class COMPUTER:
@@ -12851,106 +12882,118 @@
             def start_windows_service(name: str, computer_name: str) -> bool | None:
                 return PIH.EXECUTOR.start_windows_service(name, computer_name)
 
             @staticmethod
             def stop_windows_service(name: str, computer_name: str) -> bool | None:
                 return PIH.EXECUTOR.stop_windows_service(name, computer_name)
 
-        class MARK:
+        class DOOR:
+            
             @staticmethod
-            def door_operation(door_name: str, operation_name: str) -> bool:
-                return DataTool.rpc_unrepresent(
+            def operation(name: str, operation_name: str) -> bool:
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.door_operation,
-                        (door_name, operation_name),
+                        (name, operation_name),
                     )
                 )
+                
+            @staticmethod
+            def open(name: str) -> bool:
+                return PIH.ACTION.DOOR.operation(name, "open")
+                
+            @staticmethod
+            def close(name: str) -> bool:
+                return PIH.ACTION.DOOR.operation(name, "close")
+
+
+        class MARK:
 
             @staticmethod
             def create(
                 full_name: FullName,
                 person_division_id: int,
                 tab_number: str,
                 telephone: str | None = None,
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_mark,
                         (full_name, person_division_id, tab_number, telephone),
                     )
                 )
 
             @staticmethod
             def set_full_name_by_tab_number(
                 full_name: FullName, tab_number: str
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_full_name_by_tab_number,
                         (full_name, tab_number),
                     )
                 )
 
             @staticmethod
             def set_telephone_by_tab_number(telephone: str, tab_number: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_telephone_by_tab_number,
                         (telephone, tab_number),
                     )
                 )
 
             @staticmethod
             def make_as_free_by_tab_number(tab_number: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.make_mark_as_free_by_tab_number, tab_number
                     )
                 )
 
             @staticmethod
             def make_as_temporary(temporary_mark: Mark, owner_mark: Mark) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.make_mark_as_temporary,
                         (temporary_mark.TabNumber, owner_mark.TabNumber),
                     )
                 )
 
             @staticmethod
             def remove(mark: Mark) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.remove_mark_by_tab_number, mark.TabNumber
                     )
                 )
 
         class DOCUMENTS:
             @staticmethod
             def create_statistics_chart(type: STATISTICS.Types) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_statistics_chart, (type.name,)
                     )
                 )
 
             @staticmethod
             def save_xlsx(
-                title: str, result: Result[list[dict[str, Any]]], path: str
+                title: str, result: Result[list[strdict]], path: str
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.save_xlsx,
                         (title, result.fields.list, result.data, path),
                     )
                 )
 
             @staticmethod
             def save_base64_as_image(path: str, content: str) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.save_base64_as_image, (path, content)
                     )
                 )
 
             @staticmethod
             def create_for_user(
@@ -12959,16 +13002,16 @@
                 tab_number: str,
                 pc: LoginPasswordPair | None,
                 polibase: LoginPasswordPair | None,
                 email: LoginPasswordPair,
             ) -> bool:
                 locale.setlocale(locale.LC_ALL, "ru_RU")
                 date_now = datetime.now().date()
-                date_now_string = f"{date_now.day} {calendar.month_name[date_now.month]} {date_now.year}"
-                return DataTool.rpc_unrepresent(
+                date_now_string = js((date_now.day, calendar.month_name[date_now.month], date_now.year))
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_user_document,
                         (
                             path,
                             date_now_string,
                             ADDRESSES.SITE_ADDRESS,
                             j((CONST.SITE_PROTOCOL, ADDRESSES.SITE_ADDRESS)),
@@ -12981,29 +13024,29 @@
                         ),
                     )
                 )
 
         class WORKSTATION:
             @staticmethod
             def reboot(host: str | None = None, force: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(ServiceCommands.reboot, (host, force))
                 )
 
             @staticmethod
             def shutdown(host: str | None = None, force: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(ServiceCommands.shutdown, (host, force))
                 )
 
             @staticmethod
             def kill_process(
                 name_or_pid: str | int, host: str, via_standart_tools: bool = True
             ) -> bool:
-                return DataTool.rpc_unrepresent(
+                return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.kill_process,
                         (name_or_pid, host, via_standart_tools),
                     )
                 )
 
             @staticmethod
@@ -13121,15 +13164,15 @@
     D_C = D.CHECK
     D_STAT = D.STATISTICS
     D_U = D.USER
     D_J = D.JOURNAL
     A = root.ACTION
     A_F = A.FILES
 
-    A_D = A.DOCUMENTS
+    A_DOC = A.DOCUMENTS
     A_SSH = A.SSH
     A_QR = A.QR_CODE
     A_IND = A.INDICATION
     A_IND_CT = A_IND.CT
     A_IND_CH = A_IND.CHILLER
     ME = root.MESSAGE
     ME_P = ME.POLIBASE
@@ -13189,14 +13232,15 @@
     C_ME_WH = C_ME.WHATSAPP
     C_ME_WH_W = C_ME_WH.WAPPI
     C_N = C.NOTES
     C_J = C.JOURNALS
     C_EML = C.EMAIL
     C_RCG = C.RECOGNIZE
     #
+    A_DR = A.DOOR
     A_M = A.MARK
     A_COMP = A.COMPUTER
     R_M = R.MARK
     R_U = R.USER
     R_F = R.FILES
     R_TT = R.TIME_TRACKING
     A_U = A.USER
@@ -13333,15 +13377,15 @@
 def delay(action: Callable[[], None], value: float = 1.0, block: bool = False) -> None:
     def action_support() -> None:
         if value > 0:
             sleep(value)
         action()
 
     if block:
-        action_support
+        action_support()
     else:
         PIHThread(action_support)
 
 
 def thread(
     value: Callable,
     checker: Callable | None = None,
```

### Comparing `pih-0.33/pih/rpc/__init__.py` & `pih-0.34/pih/rpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                 for sc in self.subscriber_information_map:
                     for service_information_name in self.subscriber_information_map[sc]:
                         subscriber_information: SubscriberInformation = (
                             self.subscriber_information_map[sc][
                                 service_information_name
                             ]
                         )
-                        DataTool.rpc_unrepresent(
+                        DataTool.rpc_decode(
                             RPC.call_service(
                                 subscriber_information.service_information,
                                 SC.unsubscribe,
                                 (sc, subscriber_information.name),
                             )
                         )
                 self.subscriber_information_map = defaultdict(dict)
@@ -302,15 +302,15 @@
                         and subscriber_information.enabled
                     ):
                         subscriber_information.available = RPC.check_availability(
                             service_information
                         )
                         if subscriber_information.available:
                             out_result = ParameterList(
-                                DataTool.rpc_unrepresent(
+                                DataTool.rpc_decode(
                                     RPC.call_service(
                                         service_information,
                                         sc,
                                         (
                                             in_result,
                                             SubscribtionResult(
                                                 None,
@@ -444,19 +444,19 @@
             if DEBUG:
                 from pih import A
             else:
                 A = sys.modules["pih.pih"].A
             parameters = command.parameters
 
             if ne(parameters):
-                parameters = DataTool.rpc_unrepresent(parameters)
+                parameters = DataTool.rpc_decode(parameters)
             RPC.context = context
             result: Any = self.internal_call_handler(command.name, parameters, context)
             if n(context.code()):
-                return pb2.rpcCommandResult(data=DataTool.rpc_represent(result)) # type: ignore
+                return pb2.rpcCommandResult(data=DataTool.rpc_encode(result)) # type: ignore
             return result
 
     class Service(IService):
         MAX_WORKERS: int = 10
 
         def __init__(self):
             self.description: ServiceDescription | None = None
@@ -663,15 +663,15 @@
             if DEBUG:
                 from pih import A
             else:
                 A = sys.modules["pih.pih"].A
             for service_description in self.subscribtions_map:
                 for sc in self.subscribtions_map[service_description]:
                     if sc in command_list:
-                        DataTool.rpc_unrepresent(
+                        DataTool.rpc_decode(
                             RPC.call_service(
                                 service_description, SC.unsubscribe, (self.description,)
                             )
                         )
 
         def unsubscribe_all(
             self, service_role_or_description: ServiceRoles | ServiceDescriptionBase
@@ -762,15 +762,15 @@
                 ):
                     if sc == SC.ping:
                         timeout = CONST_RPC.TIMEOUT_FOR_PING
                     else:
                         timeout = CONST_RPC.TIMEOUT
             return (
                 RPC.CommandClient(service_host, service_port)  # type: ignore
-                .call_command(sc.name, DataTool.rpc_represent(parameters), timeout)
+                .call_command(sc.name, DataTool.rpc_encode(parameters), timeout)
                 .data
             )
         except grpc.RpcError as exception:
             code: tuple = exception.code()  # type: ignore
             details: str = j(
                 (
                     "Service role name: ",
```

### Comparing `pih-0.33/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.34/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.34/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih/tools/__init__.py` & `pih-0.34/pih/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,23 @@
 
 def nnd(value: Any) -> dict:
     return value
 
 def nns(value: Any) -> str:
     return value
 
+def nnb(value: Any) -> bytes:
+    return value
+
 def nni(value: Any) -> int:
     return value
 
+def nndt(value: Any) -> datetime:
+    return value
+
 def nnf(value: Any) -> float:
     return value
 
 def jnl(value: tuple[Any, ...] | list[Any]) -> str:
     return j(value, nl())
 
 
@@ -286,32 +292,32 @@
         if n(data):
             return default_value
         if len(data) <= index:
             return default_value
         return data[index]
 
     @staticmethod
-    def rpc_represent(data: dict | None, ensure_ascii: bool = True) -> str | None:
+    def rpc_encode(data: dict | None, ensure_ascii: bool = True) -> str | None:
         return (
             None
             if n(data)
             else json.dumps(data, cls=PIHEncoder, ensure_ascii=ensure_ascii)
         )
 
     @staticmethod
-    def rpc_unrepresent(value: str | None) -> dict[str, Any] | None:
+    def rpc_decode(value: str | None) -> dict[str, Any] | None:
         return None if e(value) else json.loads(value)
 
     @staticmethod
     def to_result(
         result_string: str | None,
         class_type_holder: Any | Callable[[Any], Any] | None = None,
         first_data_item: bool = False,
     ) -> Result[Any]:
-        result_object: dict[str, Any] | None = DataTool.rpc_unrepresent(result_string)
+        result_object: dict[str, Any] | None = DataTool.rpc_decode(result_string)
         if n(result_object):
             return Result(None, None)
         data: dict = result_object["data"]  # type: ignore
         data = DataTool.get_first_item(data) if first_data_item else data
 
         def fill_data_with(item: Any) -> Any:
             if e(class_type_holder):
@@ -466,15 +472,15 @@
                 lambda item: DataTool.fill_data_from_source(class_type(), item),
                 source if isinstance(source, list) else source.values(),
             )
         )
 
     @staticmethod
     def fill_data_from_rpc_str(data: T, source: str) -> T:
-        return DataTool.fill_data_from_source(data, DataTool.rpc_unrepresent(source))
+        return DataTool.fill_data_from_source(data, DataTool.rpc_decode(source))
 
     @staticmethod
     def get_first_item(
         value: list[T] | T | dict[str, Any], default_value: Any = None
     ) -> T | Any:
         if e(value):
             return default_value
@@ -856,15 +862,15 @@
         return result
 
 
 n = DataTool.is_none
 nn = DataTool.is_not_none
 
 
-def lw(value: str | list[str] | tuple[str, ...] | None) -> str:
+def lw(value: str | list[str] | tuple[str, ...] | None) -> str | list[str] | tuple[str, ...]:
     if n(value):
         return ""
     if isinstance(value, str):
         return value.lower()
     return DataTool.map(str.lower, value)
```

### Comparing `pih-0.33/pih/tools/service.py` & `pih-0.34/pih/tools/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from pih.consts import CONST
 from pih.consts.service_roles import ServiceRoles
 from pih.tools import NetworkTool, OSTool, j, e, n
-from pih.consts import SPLITTER, ISOLATED_ARG_NAME
 from pih.consts.service import EVENT_LISTENER_NAME_PREFIX, SUPPORT_NAME_PREFIX
-from pih.collections.service import ServiceDescriptionBase, ServiceInformation, ServiceDescription
+from pih.collections.service import (
+    ServiceDescriptionBase,
+    ServiceInformation,
+    ServiceDescription,
+)
 
 
 from enum import Enum
 
 
 class ServiceTool:
 
@@ -16,34 +20,30 @@
 
     @staticmethod
     def is_service_as_support(description: ServiceDescriptionBase) -> bool:
         return description.name.find(SUPPORT_NAME_PREFIX) == 0
 
 
 class ServiceAdminTool:
-    
-    service_collection: dict[
-                ServiceDescriptionBase, ServiceInformation
-            ] = {}
-    
+
+    service_collection: dict[ServiceDescriptionBase, ServiceInformation] = {}
+
     @staticmethod
     def remove_service_from_service_collection(value: ServiceDescriptionBase) -> None:
         if value in ServiceAdminTool.service_collection:
             del ServiceAdminTool.service_collection[value]
-            
+
     @staticmethod
     def clear_service_collection() -> None:
         ServiceAdminTool.service_collection = {}
-            
+
     @staticmethod
-    def get_service_collection() -> dict[
-                ServiceDescriptionBase, ServiceInformation
-            ]:
+    def get_service_collection() -> dict[ServiceDescriptionBase, ServiceInformation]:
         return ServiceAdminTool.service_collection
-    
+
     @staticmethod
     def update_service_information(
         value: ServiceDescriptionBase | list[ServiceDescriptionBase],
         add: bool = True,
         overwrite: bool = False,
     ) -> None:
         if not isinstance(value, list):
@@ -52,15 +52,15 @@
             ServiceAdminTool.service_collection = {}
         for item in value:
             if add:
                 ServiceAdminTool.service_collection[item] = item
             else:
                 if item in ServiceAdminTool.service_collection:
                     del ServiceAdminTool.service_collection[item]
-                    
+
     @staticmethod
     def create_port(
         service_role_or_description: ServiceRoles | ServiceDescriptionBase,
     ) -> int:
         return (
             ServiceRoleTool.service_description(service_role_or_description).port
             or NetworkTool.next_free_port()
@@ -77,27 +77,27 @@
             OSTool.host()
             if description.isolated or e(description.host)
             else description.host
         )
 
 
 class ServiceRoleTool:
-    
+
     @staticmethod
     def service_description(
         value: Enum | str | ServiceDescriptionBase, get_source_description: bool = False
     ) -> ServiceDescriptionBase | None:
         def isolated_name(
             value: ServiceDescriptionBase | None,
         ) -> ServiceDescriptionBase | None:
             if n(value):
                 return None
             value.name = (
-                j((ISOLATED_ARG_NAME, value.name), SPLITTER)
-                if value.isolated and value.name.find(ISOLATED_ARG_NAME) == -1
+                j((CONST.ISOLATED_ARG_NAME, value.name), CONST.SPLITTER)
+                if value.isolated and value.name.find(CONST.ISOLATED_ARG_NAME) == -1
                 else value.name
             )
             return value
 
         if isinstance(value, str):
             for service_role in ServiceRoles:
                 if ServiceRoleTool.service_description(service_role).name == value:
```

### Comparing `pih-0.33/pih/widgets.py` & `pih-0.34/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.33/pih.egg-info/SOURCES.txt` & `pih-0.34/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

