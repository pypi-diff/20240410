# Comparing `tmp/pih-ad-0.13.tar.gz` & `tmp/pih-ad-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ad-0.13.tar", last modified: Wed Mar 13 12:10:26 2024, max compression
+gzip compressed data, was "pih-ad-0.14.tar", last modified: Wed Apr 10 01:30:39 2024, max compression
```

## Comparing `pih-ad-0.13.tar` & `pih-ad-0.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 12:10:26.174066 pih-ad-0.13/
-drwxrwxrwx   0        0        0        0 2024-03-13 12:10:25.752234 pih-ad-0.13/ActiveDirectoryService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.13/ActiveDirectoryService/__init__.py
--rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.13/ActiveDirectoryService/__main__.py
--rw-rw-rw-   0        0        0    18340 2024-03-11 05:53:10.000000 pih-ad-0.13/ActiveDirectoryService/api.py
--rw-rw-rw-   0        0        0     1601 2024-03-13 12:10:18.000000 pih-ad-0.13/ActiveDirectoryService/const.py
--rw-rw-rw-   0        0        0    15355 2024-03-11 05:44:07.000000 pih-ad-0.13/ActiveDirectoryService/service.py
--rw-rw-rw-   0        0        0      340 2024-03-13 12:10:26.127192 pih-ad-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-13 12:10:26.095943 pih-ad-0.13/pih_ad.egg-info/
--rw-rw-rw-   0        0        0      340 2024-03-13 12:10:25.000000 pih-ad-0.13/pih_ad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-03-13 12:10:25.000000 pih-ad-0.13/pih_ad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 12:10:25.000000 pih-ad-0.13/pih_ad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-03-13 12:10:25.000000 pih-ad-0.13/pih_ad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-03-13 12:10:25.000000 pih-ad-0.13/pih_ad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-03-13 12:10:25.000000 pih-ad-0.13/pih_ad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 12:10:26.189690 pih-ad-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:30:39.686246 pih-ad-0.14/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:30:39.133348 pih-ad-0.14/ActiveDirectoryService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.14/ActiveDirectoryService/__init__.py
+-rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.14/ActiveDirectoryService/__main__.py
+-rw-rw-rw-   0        0        0    18006 2024-04-09 23:50:16.000000 pih-ad-0.14/ActiveDirectoryService/api.py
+-rw-rw-rw-   0        0        0     1601 2024-04-09 23:21:36.000000 pih-ad-0.14/ActiveDirectoryService/const.py
+-rw-rw-rw-   0        0        0    15355 2024-03-11 05:44:07.000000 pih-ad-0.14/ActiveDirectoryService/service.py
+-rw-rw-rw-   0        0        0      340 2024-04-10 01:30:39.670626 pih-ad-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:30:39.592501 pih-ad-0.14/pih_ad.egg-info/
+-rw-rw-rw-   0        0        0      340 2024-04-10 01:30:38.000000 pih-ad-0.14/pih_ad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-10 01:30:38.000000 pih-ad-0.14/pih_ad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:30:38.000000 pih-ad-0.14/pih_ad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-10 01:30:38.000000 pih-ad-0.14/pih_ad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-10 01:30:38.000000 pih-ad-0.14/pih_ad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-10 01:30:38.000000 pih-ad-0.14/pih_ad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:30:39.701871 pih-ad-0.14/setup.cfg
```

### Comparing `pih-ad-0.13/ActiveDirectoryService/api.py` & `pih-ad-0.14/ActiveDirectoryService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from collections import defaultdict
+import os
+import pythoncom
 import pywintypes
+import win32security
+from typing import Any
+from wmi import WMI, x_wmi
 from pyad import pyadutils
 from pyad.aduser import ADUser
 from pyad.adquery import ADQuery
+from collections import defaultdict
 from pyad.adcomputer import ADComputer
 from pyad.adcontainer import ADContainer
 from pyad.adgroup import ADObject, ADGroup
 
-import os
-import pythoncom
-import win32security
-from typing import Any
-from wmi import WMI, x_wmi
-
-
 import ipih
 
 from pih import A
 from pih.consts.errors import NotAccesable
 from pih.collections import FullName, User
 from ActiveDirectoryService.const import *
 from pih.tools import if_else, j, n, nn, lw, ne
@@ -358,15 +356,15 @@
             prefixed_name = j((prefix, name), "=")
             return self._ldap_adsi_obj.Create(type, prefixed_name)
 
         def create_user(
             self, login, name, password, upn_suffix, optional_attributes={}
         ):
             try:
-                upn = j((login, upn_suffix), A.CT.EMAIL.SPLITTER)
+                upn = j((login, upn_suffix), A.CT.)
                 obj = self.__create_user_object(name)
                 obj.Put(
                     "sAMAccountName", optional_attributes.get("sAMAccountName", login)
                 )
                 obj.Put("userPrincipalName", upn)
                 obj.SetInfo()
                 pyadobj = ADUser.from_com_object(obj)
@@ -396,24 +394,24 @@
                     result_group_list[group.dn] = group
             user_container: ActiveDirectoryApi.UserContainer = (
                 ActiveDirectoryApi.UserContainer.from_dn(
                     A.D_Ex.container_dn_from_dn(templated_user_dn)
                 )
             )
             name = A.D.fullname_to_string(full_name)
-            new_user: ADUser = user_container.create_user(
+            new_user: ADUser | None = user_container.create_user(
                 login,
                 name,
                 password,
                 A.CT_AD.DOMAIN_MAIN,
                 optional_attributes={
                     "givenName": A.D.to_given_name(full_name),
                     "sn": full_name.last_name,
                     "userPrincipalName": A.D_F.user_principal_name(login),
-                    "homeDirectory": A.PTH.adapt_for_windows(
+                    "homeDirectory": A.PTH.for_windows(
                         j((A.PTH_U.HOME_FOLDER_FULL, login), "\\")
                     ),
                     "displayName": name,
                     "homeDrive": A.CT_AD.USER_HOME_FOLDER_DISK,
                     "mail": email,
                     "description": description,
                     "telephonenumber": telephone,
@@ -443,27 +441,14 @@
         @staticmethod
         def user_remove(user_dn: str) -> bool:
             try:
                 ADUser.from_dn(user_dn).delete()
                 return True
             except:
                 return False
-
-        @staticmethod
-        def create_user_in_container(
-            container_dn: str,
-            full_name: FullName,
-            login: str,
-            password: str,
-            description: str,
-            telephone: str,
-            email: str,
-        ) -> bool:
-            return True
-
         @staticmethod
         def user_set_telephone_number(user_dn: str, telephone: str) -> bool:
             ActiveDirectoryApi.user_set_telephone_number(user_dn, telephone)
             return True
 
         @staticmethod
         def user_set_password(user_dn: str, password: str) -> bool:
@@ -474,8 +459,8 @@
         def user_move(user_dn: str, container_dn: str) -> bool:
             ActiveDirectoryApi.user_move(user_dn, container_dn)
             return True
 
         @staticmethod
         def user_set_status(user_dn: str, status: str, container_dn: str) -> bool:
             ActiveDirectoryApi.user_set_dn(user_dn, status, container_dn)
-            return True
+            return True
```

### Comparing `pih-ad-0.13/ActiveDirectoryService/const.py` & `pih-ad-0.14/ActiveDirectoryService/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "ActiveDirectory"
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 PACKAGES: tuple[str, ...] = ("pyad", "pywin32", "wmi")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Active directory service",
     host=HOST.NAME,
```

### Comparing `pih-ad-0.13/ActiveDirectoryService/service.py` & `pih-ad-0.14/ActiveDirectoryService/service.py`

 * *Files identical despite different names*

