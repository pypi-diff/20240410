# Comparing `tmp/amino.light.py-0.1.1.tar.gz` & `tmp/amino.light.py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.1.tar", last modified: Mon Apr  8 13:13:37 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.2.tar", last modified: Wed Apr 10 17:27:41 2024, max compression
```

## Comparing `amino.light.py-0.1.1.tar` & `amino.light.py-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.730595 amino.light.py-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.677594 amino.light.py-0.1.1/AminoLightPy/
--rw-rw-rw-   0        0        0      296 2024-04-08 13:05:43.000000 amino.light.py-0.1.1/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0     8472 2024-04-03 00:57:53.000000 amino.light.py-0.1.1/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    66358 2024-04-08 10:39:29.000000 amino.light.py-0.1.1/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2643 2024-04-08 13:03:57.000000 amino.light.py-0.1.1/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.678593 amino.light.py-0.1.1/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.1/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.692596 amino.light.py-0.1.1/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1352 2024-04-08 09:38:49.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    94998 2024-04-08 09:43:52.000000 amino.light.py-0.1.1/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    17215 2024-04-08 13:05:17.000000 amino.light.py-0.1.1/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    71961 2024-04-08 12:57:01.000000 amino.light.py-0.1.1/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1812 2024-04-08 13:13:37.729594 amino.light.py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1019 2024-04-04 18:43:15.000000 amino.light.py-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 13:13:37.728593 amino.light.py-0.1.1/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     1812 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-08 13:13:37.000000 amino.light.py-0.1.1/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 13:13:37.739600 amino.light.py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1295 2024-04-08 13:13:31.000000 amino.light.py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.233783 amino.light.py-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.155768 amino.light.py-0.1.2/AminoLightPy/
+-rw-rw-rw-   0        0        0      296 2024-04-08 13:05:43.000000 amino.light.py-0.1.2/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0    17388 2024-04-10 00:15:18.000000 amino.light.py-0.1.2/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    72454 2024-04-10 13:49:30.000000 amino.light.py-0.1.2/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2643 2024-04-08 13:03:57.000000 amino.light.py-0.1.2/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.157766 amino.light.py-0.1.2/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.2/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.169774 amino.light.py-0.1.2/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    32075 2024-04-09 21:58:19.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1354 2024-04-09 22:00:38.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    94934 2024-04-10 12:04:03.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0    17113 2024-04-10 13:21:35.000000 amino.light.py-0.1.2/AminoLightPy/socket.py
+-rw-rw-rw-   0        0        0    75163 2024-04-10 13:49:22.000000 amino.light.py-0.1.2/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4060 2024-04-10 17:27:41.230785 amino.light.py-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3264 2024-04-10 17:23:45.000000 amino.light.py-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.225765 amino.light.py-0.1.2/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     4060 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 17:27:41.245770 amino.light.py-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-04-10 17:27:16.000000 amino.light.py-0.1.2/setup.py
```

### Comparing `amino.light.py-0.1.1/AminoLightPy/client.py` & `amino.light.py-0.1.2/AminoLightPy/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# pylint: disable=invalid-name
+
 from uuid import uuid4
-from base64 import b64encode
 from typing import BinaryIO, Union
 
-from .constants import *
+from .constants import api, upload_media, AminoSession
 from .socket import Callbacks, SocketHandler, SocketRequests
 from .lib.util import exceptions, objects, helpers, self_deviceId
 
 
 #@dorthegra/IDörthe#8835 thanks for support!
 
 class Client(Callbacks, SocketHandler, SocketRequests):
@@ -14,26 +15,30 @@
         self.api = api
         self.authenticated = False
         self.session = AminoSession()
         self.device_id = self.session.headers["NDCDEVICEID"]
 
         self.socket_enabled = socket_enabled
         if socket_enabled:
-            handler = SocketHandler.__init__(self, self, socketDebugging)
-            SocketRequests.__init__(self, handler)
+            SocketHandler.__init__(self, self, socketDebugging)
+            SocketRequests.__init__(self)
             Callbacks.__init__(self)
 
         self.session.proxies = proxies
 
         self.sid = None
-        self.profile: objects.UserProfile = objects.UserProfile(None).UserProfile
+        self.profile = objects.UserProfile(None).UserProfile
         self.profile.session = self.session
 
 
     def parse_headers(self, data: str = None) -> dict:
+        """
+        **Returns**
+            - Headers. For support old custom requests
+        """
         base_headers: dict = self.session.headers
         if data:
             base_headers["NDC-MSG-SIG"] = helpers.signature(data)
 
         return base_headers
 
 
@@ -44,16 +49,16 @@
         **Parameters**
             - **SID** : SID of the account
         """
         userId = helpers.sid_to_uid(SID)
         self.authenticated = True
         self.sid = SID
 
-        self.profile: objects.UserProfile = objects.UserProfile({"uid": userId}).UserProfile
-    
+        self.profile = objects.UserProfile({"uid": userId}).UserProfile
+
         self.session.headers.update({
             "NDCAUTH": f"sid={self.sid}",
             "AUID": self.profile.userId
             })
 
         self.profile.session = self.session
 
@@ -67,15 +72,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         if self_device:
             self.session.headers["NDCDEVICEID"] = self_deviceId(email)
 
         data = {
             "email": email,
             "secret": f"0 {password}",
@@ -84,15 +89,15 @@
             "v": 2
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
         self.sid = json["sid"]
-        self.profile: objects.UserProfile = objects.UserProfile(json["userProfile"]).UserProfile
+        self.profile = objects.UserProfile(json["userProfile"]).UserProfile
 
         self.session.headers.update({
             "NDCAUTH": f"sid={self.sid}",
             "AUID": self.profile.userId
         })
 
         self.profile.session = self.session
@@ -109,15 +114,15 @@
         **Parameters**
             - **phoneNumber** : Phone number of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         if self_device:
             self.session.headers["NDCDEVICEID"] = self_deviceId(phoneNumber)
 
         data = {
             "phoneNumber": phoneNumber,
             "v": 2,
@@ -128,15 +133,15 @@
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
         self.sid = json["sid"]
 
-        self.profile: objects.UserProfile = objects.UserProfile(json["userProfile"]).UserProfile
+        self.profile = objects.UserProfile(json["userProfile"]).UserProfile
 
         self.session.headers.update({
             "NDCAUTH": f"sid={self.sid}",
             "AUID": self.profile.userId
         })
 
         self.profile.session = self.session
@@ -152,15 +157,15 @@
 
         **Parameters**
             - **secret** : Secret of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         if self_device:
             self.session.headers["NDCDEVICEID"] = self_deviceId(secret)
 
         data = {
             "v": 2,
             "secret": secret,
@@ -170,50 +175,48 @@
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
         self.sid = json["sid"]
 
-        self.profile: objects.UserProfile = objects.UserProfile(json["userProfile"]).UserProfile
+        self.profile = objects.UserProfile(json["userProfile"]).UserProfile
 
         self.session.headers.update({
             "NDCAUTH": f"sid={self.sid}",
             "AUID": self.profile.userId
         })
 
         self.profile.session = self.session
 
         if self.socket_enabled:
             self.run_amino_socket()
 
         return json
 
-    def register(self, nickname: str, email: str, password: str, verificationCode: str, deviceId: str = None):
+    def register(self, nickname: str, email: str, password: str, verificationCode: str):
         """
         Register an account.
 
         **Parameters**
             - **nickname** : Nickname of the account.
             - **email** : Email of the account.
             - **password** : Password of the account.
             - **verificationCode** : Verification code.
             - **deviceId** : The device id being registered to.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
-        if not deviceId: deviceId = self.device_id
-
         data = {
             "secret": f"0 {password}",
-            "deviceID": deviceId,
+            "deviceID": self.device_id,
             "email": email,
             "clientType": 100,
             "nickname": nickname,
             "latitude": 0,
             "longitude": 0,
             "address": None,
             "clientCallbackURL": "narviiapp://relogin",
@@ -221,16 +224,15 @@
                 "data": {
                     "code": verificationCode
                 },
                 "type": 1,
                 "identity": email
             },
             "type": 1,
-            "identity": email,
-        }     
+            "identity": email}     
 
         response = self.session.post(f"{api}/g/s/auth/register", json=data)
         return response.json()
 
     def restore(self, email: str, password: str):
         """
         Restore a deleted account.
@@ -238,15 +240,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "secret": f"0 {password}",
             "deviceID": self.device_id,
             "email": email
         }
 
@@ -259,15 +261,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "deviceID": self.device_id,
             "clientType": 100
         }
 
         response = self.session.post(f"{api}/g/s/auth/logout", json=data)
@@ -294,26 +296,27 @@
             - **age** : Age of the account. Minimum is 13.
             - **gender** : Gender of the account.
                 - ``Male``, ``Female`` or ``Non-Binary``
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if gender.lower() == "male": gender = 1
-        elif gender.lower() == "female": gender = 2
-        elif gender.lower() == "non-binary": gender = 255
-        else: raise exceptions.SpecifyType
+        gender_mapping = {"male": 1, "female": 2, "non-binary": 255}
 
-        if age <= 12: raise exceptions.AgeTooLow
+        gender = gender.lower()
+        if gender not in gender_mapping:
+            raise exceptions.SpecifyType
+
+        age = max(13, age)
 
         data = {
             "age": age,
-            "gender": gender,
+            "gender": gender_mapping[gender],
         }
 
         response = self.session.post(f"{api}/g/s/persona/profile/basic", json=data)
         return response.status_code
 
     def verify(self, email: str, code: str):
         """
@@ -322,15 +325,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "validationContext": {
                 "type": 1,
                 "identity": email,
                 "data": {"code": code}},
             "deviceID": self.device_id,
@@ -346,15 +349,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **resetPassword** : If the code should be for Password Reset.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "identity": email,
             "type": 1,
             "deviceID": self.device_id
         }
 
@@ -372,15 +375,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         data = {
             "type": 1,
             "identity": email,
             "data": {"code": code},
             "deviceID": self.device_id
@@ -396,15 +399,15 @@
 
         **Parameters**
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         data = {
             "deviceID": self.device_id,
             "secret": f"0 {password}"
         }
 
@@ -419,15 +422,15 @@
             - **email** : Email of the account.
             - **password** : Password of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         data = {
             "updateSecret": f"0 {password}",
             "emailValidationContext": {
                 "data": {
                     "code": code
@@ -442,107 +445,163 @@
         }
 
         response = self.session.post(f"{api}/g/s/auth/reset-password", json=data)
         return response.status_code
 
 
     def get_account_info(self):
+        """
+        Information of an this account.
+
+        **Returns**
+            - **Success** : :meth:`User Object <AminoLightPy.lib.util.objects.UserProfile>`
+
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         response = self.session.get(f"{api}/g/s/account")
         return objects.UserProfile(response.json()["account"]).UserProfile
 
     def handle_socket_message(self, data):
+        "Adapter between receiving messages and processing them"
         return self.resolve(data)
 
     def get_eventlog(self):
-        response = self.session.get(f"{api}/g/s/eventlog/profile?language=en")
+        """
+        Information of an events.
+
+        **Returns**
+            - **Success** : :meth:`dict`
+
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+        params = {"language": "en"}
+        response = self.session.get(f"{api}/g/s/eventlog/profile", params=params)
         return response.json()
 
     def sub_clients(self, start: int = 0, size: int = 25):
         """
         List of Communities the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <AminoLightPy.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if not self.authenticated: raise exceptions.NotLoggedIn
+        if not self.authenticated:
+            raise exceptions.NotLoggedIn
         response = self.session.get(f"{api}/g/s/community/joined?v=1&start={start}&size={size}")
         return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     def sub_clients_profile(self, start: int = 0, size: int = 25):
-        if not self.authenticated: raise exceptions.NotLoggedIn
+        """
+        List of profiles in communities.
+
+        **Parameters**
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
+
+        **Returns**
+            - **Success** : :meth:`list<dict>`
+
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+        if not self.authenticated:
+            raise exceptions.NotLoggedIn
         response = self.session.get(f"{api}/g/s/community/joined?v=1&start={start}&size={size}")
         return response.json()["userInfoInCommunities"]
 
     def get_user_info(self, userId: str):
         """
         Information of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+            - **Success** : :meth:`User Object <AminoLightPy.lib.util.objects.UserProfile>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/user-profile/{userId}")
         return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
     def get_chat_threads(self, start: int = 0, size: int = 25):
         """
         List of Chats the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <AminoLightPy.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        response = self.session.get(f"{api}/g/s/chat/thread?type=joined-me&start={start}&size={size}")
+        params = {
+            "start": start,
+            "size": size,
+            "type": "joined-me"
+        }
+        response = self.session.get(f"{api}/g/s/chat/thread", params=params)
         return objects.ThreadList(response.json()["threadList"]).ThreadList
 
     def get_chat_thread(self, chatId: str):
         """
         Get the Chat Object from an Chat ID.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+            - **Success** : :meth:`Chat Object <AminoLightPy.lib.util.objects.Thread>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/chat/thread/{chatId}")
         return objects.Thread(response.json()["thread"]).Thread
 
     def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{api}/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2")
+        """
+        List of users in a chat.
+
+        **Parameters**
+            - **chatId** (str): ID of the chat.
+            - *start* (int, optional): The index from which to start the list. Defaults to 0.
+            - *size* (int, optional): The size of the list. Defaults to 25.
+
+        **Returns**
+            - **Success** : :meth:`User List <AminoLightPy.lib.util.objects.UserProfileList>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+        params = {
+            "start": start,
+            "size": size,
+            "type": "default",
+            "cv": "1.2"
+        }
+
+        response = self.session.get(f"{api}/g/s/chat/thread/{chatId}/member", params=params)
         return objects.UserProfileList(response.json()["memberList"]).UserProfileList
 
     def join_chat(self, chatId: str):
         """
         Join an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}")
         return response.status_code
 
     def leave_chat(self, chatId: str):
         """
@@ -550,256 +609,309 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}")
+        userId = self.profile.userId
+        response = self.session.delete(f"{api}/g/s/chat/thread/{chatId}/member/{userId}")
         return response.status_code
 
-    def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
+    def start_chat(self, userId: Union[str, list], message: str,
+            title: str = None, content: str = None,
+            isGlobal: bool = False, publishToGlobal: bool = False):
         """
         Start an Chat with an User or List of Users.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **message** : Starting Message.
             - **title** : Title of Group Chat.
             - **content** : Content of Group Chat.
             - **isGlobal** : If Group Chat is Global.
             - **publishToGlobal** : If Group Chat should show in Global.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if isinstance(userId, str): userIds = [userId]
-        elif isinstance(userId, list): userIds = userId
-        elif isinstance(userId, tuple): userIds = userId
-        else: raise exceptions.WrongType
+        if isinstance(userId, (str, list, tuple)):
+            userIds = list(userId)
+        else:
+            raise exceptions.WrongType
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
+            "type": 2 if isGlobal else 0,
+            "publishToGlobal": 1 if publishToGlobal else 0
         }
 
-        if isGlobal is True:
-            data["type"] = 2
+        if isGlobal:
             data["eventSource"] = "GlobalComposeMenu"
-        else: data["type"] = 0
-
-        if publishToGlobal is True: data["publishToGlobal"] = 1
-        else: data["publishToGlobal"] = 0
-
 
         response = self.session.post(f"{api}/g/s/chat/thread", json=data)
         return objects.Thread(response.json()["thread"]).Thread
 
+
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
         """
         Invite a User or List of Users to a Chat.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if isinstance(userId, str): userIds = [userId]
-        elif isinstance(userId, list): userIds = userId
-        elif isinstance(userId, tuple): userIds = userId
-        else: raise exceptions.WrongType
+        if not isinstance(userId, (str, list)):
+            raise exceptions.WrongType
+
+        userIds = list(userId) if isinstance(userId, str) else userId
 
         data = {
             "uids": userIds
         }
 
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/invite", json=data)
         return response.status_code
 
+
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
-        if allowRejoin: allowRejoin = 1
-        if not allowRejoin: allowRejoin = 0
+        """
+        Kicks a user from a chat.
+
+        **Parameters**
+            - **userId** (str): ID of the user to be kicked.
+            - **chatId** (str): ID of the chat from which the user is to be kicked.
+            - *allowRejoin* (bool, optional): Whether the user is allowed to rejoin the chat. Defaults to True.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+
+        params = {"allowRejoin": int(allowRejoin)}
 
-        response = self.session.delete(f"{api}/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}")
+        response = self.session.delete(
+            url=f"{api}/g/s/chat/thread/{chatId}/member/{userId}",
+            params=params
+        )
         return response.status_code
 
     def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
         """
         List of Messages from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+            - **Success** : :meth:`Message List <AminoLightPy.lib.util.objects.MessageList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if not pageToken: url = f"{api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
-        else: url = f"{api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
+        params = {
+            "pagingType": "t",
+            "size": size,
+        }
+        if pageToken:
+            params["pageToken"] = pageToken
 
-        response = self.session.get(url)
+        response = self.session.get(f"{api}/g/s/chat/thread/{chatId}/message", params=params)
         return objects.GetMessages(response.json()).GetMessages
 
     def get_message_info(self, chatId: str, messageId: str):
         """
         Information of an Message from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - **messageId** : ID of the Message.
 
         **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+            - **Success** : :meth:`Message Object <AminoLightPy.lib.util.objects.Message>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/chat/thread/{chatId}/message/{messageId}")
         return objects.Message(response.json()["message"]).Message
 
     def get_community_info(self, comId: int):
         """
         Information of an Community.
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
+            - **Success** : :meth:`Community Object <AminoLightPy.lib.util.objects.Community>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount")
         return objects.Community(response.json()["community"]).Community
 
     def search_community(self, aminoId: str):
         """
         Search a Community byt its Amino ID.
 
         **Parameters**
             - **aminoId** : Amino ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <AminoLightPy.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/search/amino-id-and-link?q={aminoId}")
         result = response.json()["resultList"]
-        if len(result) == 0: raise exceptions.CommunityNotFound(aminoId)
-        else: return objects.CommunityList([com["refObject"] for com in result]).CommunityList
+        if not result:
+            raise exceptions.CommunityNotFound(aminoId)
+        return objects.CommunityList([com["refObject"] for com in result]).CommunityList
 
     def get_user_following(self, userId: str, start: int = 0, size: int = 25):
         """
         List of Users that the User is Following.
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <AminoLightPy.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/user-profile/{userId}/joined?start={start}&size={size}")
         return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
         """
         List of Users that are Following the User.
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <AminoLightPy.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/user-profile/{userId}/member?start={start}&size={size}")
         return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_blocked_users(self, start: int = 0, size: int = 25):
         """
         List of Users that the User Blocked.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`Users List <AminoLightPy.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/block?start={start}&size={size}")
         return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
+        """
+        Get information about a blog, wiki, quiz, or file.
+
+        Parameters:
+            blogId (str): ID of the blog.
+            wikiId (str): ID of the wiki.
+            quizId (str): ID of the quiz.
+            fileId (str): ID of the file.
+
+        Returns:
+            object: Information about the blog, wiki, quiz, or file.
+        """
         if blogId or quizId:
-            if quizId is not None: blogId = quizId
+            blogId = quizId if quizId is not None else blogId
             response = self.session.get(f"{api}/g/s/blog/{blogId}")
             return objects.GetBlogInfo(response.json()).GetBlogInfo
 
-        elif wikiId:
+        if wikiId:
             response = self.session.get(f"{api}/g/s/item/{wikiId}")
-            return objects.GetBlogInfo(response.json()).GetWikiInfo
+            return objects.GetWikiInfo(response.json()).GetWikiInfo
 
-        elif fileId:
+        if fileId:
             response = self.session.get(f"{api}/g/s/shared-folder/files/{fileId}")
             return objects.SharedFolderFile(response.json()["file"]).SharedFolderFile
 
-        else: raise exceptions.SpecifyType()
+        raise exceptions.SpecifyType()
+
 
-    def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
-        if sorting == "newest": sorting = "newest"
-        elif sorting == "oldest": sorting = "oldest"
-        elif sorting == "top": sorting = "vote"
-        else: raise exceptions.WrongType(sorting)
+    def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None,
+            fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
+        """
+        Get comments from a blog, wiki, quiz, or file.
+
+        Parameters:
+            blogId (str): ID of the blog.
+            wikiId (str): ID of the wiki.
+            quizId (str): ID of the quiz.
+            fileId (str): ID of the file.
+            sorting (str): Sorting order of comments. Can be "newest", "oldest", or "top".
+            start (int): Starting index of comments.
+            size (int): Number of comments to fetch.
+
+        Returns:
+            CommentList: List of comments.
+        """
+        sorting_dict = {"newest": "newest", "oldest": "oldest", "top": "vote"}
+        sorting = sorting_dict.get(sorting)
+        if sorting is None:
+            raise exceptions.WrongType(sorting)
 
         if blogId or quizId:
-            if not quizId: 
-                blogId = quizId
-            url = f"{api}/g/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}"
-        elif wikiId: url = f"{api}/g/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}"
-        elif fileId: url = f"{api}/g/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}",
-        else: raise exceptions.SpecifyType
+            blogId = quizId if not blogId else blogId
+            url = f"{api}/g/s/blog/{blogId}/comment"
+        elif wikiId:
+            url = f"{api}/g/s/item/{wikiId}/comment"
+        elif fileId:
+            url = f"{api}/g/s/shared-folder/files/{fileId}/comment"
+        else:
+            raise exceptions.SpecifyType
 
-        response = self.session.get(url)
+        params = {"sort": sorting, "start": start, "size": size}
+        response = self.session.get(url, params=params)
         return objects.CommentList(response.json()["commentList"]).CommentList
 
     def get_blocker_users(self, start: int = 0, size: int = 25):
         """
         List of Users that are Blocking the User.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List of User IDs <None>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/block/full-list?start={start}&size={size}")
         return response.json()["blockerUidList"]
 
     def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
         """
         List of Wall Comments of an User.
@@ -808,22 +920,26 @@
             - **userId** : ID of the User.
             - **sorting** : Order of the Comments.
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : :meth:`Comments List <AminoLightPy.lib.util.objects.CommentList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if sorting.lower() == "newest": sorting = "newest"
-        elif sorting.lower() == "oldest": sorting = "oldest"
-        elif sorting.lower() == "top": sorting = "vote"
-        else: raise exceptions.WrongType(sorting)
+        if sorting.lower() == "newest":
+            sorting = "newest"
+        elif sorting.lower() == "oldest":
+            sorting = "oldest"
+        elif sorting.lower() == "top":
+            sorting = "vote"
+        else:
+            raise exceptions.WrongType(sorting)
 
         response = self.session.get(f"{api}/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}")
         return objects.CommentList(response.json()["commentList"]).CommentList
 
     def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
         """
         Flag a User, Blog or Wiki.
@@ -835,18 +951,20 @@
             - **blogId** : ID of the Blog.
             - **wikiId** : ID of the Wiki.
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if reason is None: raise exceptions.ReasonNeeded
-        if flagType is None: raise exceptions.FlagTypeNeeded
+        if reason is None:
+            raise exceptions.ReasonNeeded
+        if flagType is None:
+            raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason
         }
 
         if userId:
@@ -857,23 +975,27 @@
             data["objectId"] = blogId
             data["objectType"] = 1
 
         elif wikiId:
             data["objectId"] = wikiId
             data["objectType"] = 2
 
-        else: raise exceptions.SpecifyType
+        else:
+            raise exceptions.SpecifyType
 
-        if asGuest: flg = "g-flag"
-        else: flg = "flag"
+        if asGuest:
+            flg = "g-flag"
+        else:
+            flg = "flag"
 
         response = self.session.post(f"{api}/g/s/{flg}", json=data)
         return response.status_code
 
     def check_values(self, *args):
+        "Check params in send_message metod."
         return any(arg is None for arg in args)
 
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
@@ -891,24 +1013,23 @@
             - **embedLink** : Link of the Embed.
             - **embedImage** : Image of the Embed.
             - **embedId** : ID of the Embed.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         data = {
             "type": messageType,
             "content": message
         }
-        
         if self.check_values(embedId, embedType, embedLink, embedTitle, embedContent, embedImage):
-            attachedObject = dict()
+            attachedObject = {}
 
             if embedId:
                 attachedObject["objectId"] = embedId
 
             if embedType:
                 attachedObject["objectType"] = embedType
 
@@ -919,22 +1040,21 @@
                 attachedObject["title"] = embedTitle
 
             if embedContent:
                 attachedObject["content"] = embedContent
 
             if embedImage:
                 attachedObject["mediaList"] = [[100, upload_media(self, embedImage, "image"), None]]
-
             data["attachedObject"] = attachedObject
-        
         if mentionUserIds:
             mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
             data["extensions"] = {"mentionedArray": mentions}
 
-        if replyTo: data["replyMessageId"] = replyTo
+        if replyTo:
+            data["replyMessageId"] = replyTo
 
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
             data["type"] = 3
 
         if file:
@@ -955,44 +1075,44 @@
             - **chatId** : ID of the Chat.
             - **asStaff** : If execute as a Staff member (Leader or Curator).
             - **reason** : Reason of the action to show on the Moderation History.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "adminOpName": 102,
         }
 
         if asStaff and reason:
             data["adminOpNote"] = {"content": reason}
-        
-        if not asStaff: response = self.session.delete(f"{api}/g/s/chat/thread/{chatId}/message/{messageId}")
-        else: response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/message/{messageId}/admin", json=data)
+        if not asStaff:
+            response = self.session.delete(f"{api}/g/s/chat/thread/{chatId}/message/{messageId}")
+        else:
+            response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/message/{messageId}/admin", json=data)
         return response.status_code
 
     def mark_as_read(self, chatId: str, messageId: str):
         """
         Mark a Message from a Chat as Read.
 
         **Parameters**
             - **messageId** : ID of the Message.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "messageId": messageId,
         }
-        
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/mark-as-read", json=data)
         return response.status_code
 
     def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None, title: str = None, icon: str = None, backgroundImage: str = None, content: str = None, announcement: str = None, coHosts: list = None, keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None, canTip: bool = None, viewOnly: bool = None, canInvite: bool = None, fansOnly: bool = None):
         """
         Send a Message to a Chat.
 
@@ -1013,142 +1133,147 @@
             - **publishToGlobal** : If the Chat should show on Public Chats or not.
             - **doNotDisturb** : If the Chat should Do Not Disturb or not.
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        data = dict()
-
-        if title: data["title"] = title
-        if content: data["content"] = content
-        if icon: data["icon"] = icon
-        if keywords: data["keywords"] = keywords
-        if announcement: data["extensions"] = {"announcement": announcement}
-        if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
-        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        data = {}
 
-        if publishToGlobal: data["publishToGlobal"] = 0
-        if not publishToGlobal: data["publishToGlobal"] = 1
+        if title:
+            data["title"] = title
+        if content:
+            data["content"] = content
+        if icon:
+            data["icon"] = icon
+        if keywords:
+            data["keywords"] = keywords
+        if announcement:
+            data["extensions"] = {"announcement": announcement}
+        if pinAnnouncement:
+            data["extensions"] = {"pinAnnouncement": pinAnnouncement}
+        if fansOnly:
+            data["extensions"] = {"fansOnly": fansOnly}
+        if publishToGlobal:
+            data["publishToGlobal"] = 0
+        if not publishToGlobal:
+            data["publishToGlobal"] = 1
 
         res = []
 
-        if doNotDisturb != None:
+        if doNotDisturb is not None:
             if doNotDisturb:
                 data = {"alertOption": 2}
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", json=data)
                 res.append(response.status_code)
-
             if not doNotDisturb:
                 data = {"alertOption": 1}
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", json=data)
                 res.append(response.status_code)
-
-        if pinChat != None:
+        if pinChat is not None:
             if pinChat:
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/pin", json=data)
                 res.append(response.status_code)
-
             if not pinChat:
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/unpin", json=data)
                 res.append(response.status_code)
-
-        if backgroundImage != None:
+        if backgroundImage is not None:
             data = {"media": [100, backgroundImage, None]}
-            
             response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/{self.profile.userId}/background", json=data)
             res.append(response.status_code)
-
-        if coHosts != None:
+        if coHosts is not None:
             data = {"uidList": coHosts}
-            
             response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/co-host", data=data)
             res.append(response.status_code)
-        
-        if viewOnly != None:
+        if viewOnly is not None:
             if viewOnly:
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/view-only/enable")
                 res.append(response.status_code)
 
             if not viewOnly:
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/view-only/disable")
                 res.append(response.status_code)
-
-        if canInvite != None:
+        if canInvite is not None:
             if canInvite:
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/members-can-invite/enable", json=data)
                 res.append(response.status_code)
-
             if not canInvite:
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/members-can-invite/disable", json=data)
                 res.append(response.status_code)
-
-        if canTip != None:
+        if canTip is not None:
             if canTip:
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/tipping-perm-status/enable", json=data)
                 res.append(response.status_code)
-
             if not canTip:
-                
                 response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/tipping-perm-status/disable", json=data)
                 res.append(response.status_code)
-        
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}", json=data)
         res.append(response.status_code)
 
         return res
 
     def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
+        """
+        Sends coins to a specified blog, chat, or object in the community.
+
+        **Parameters**
+            - *coins* : The number of coins to be sent.
+            - *blogId* : The ID of the blog to which the coins are to be sent. If not provided, the coins will not be sent to a blog.
+            - *chatId* : The ID of the chat to which the coins are to be sent. If not provided, the coins will not be sent to a chat.
+            - *objectId* : The ID of the object to which the coins are to be sent. If not provided, the coins will not be sent to an object.
+            - *transactionId* : The ID of the transaction. If not provided, a new transaction ID will be generated.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         url = None
-        if transactionId is None: transactionId = str(uuid4())
+        if transactionId is None:
+            transactionId = str(uuid4())
 
         data = {
             "coins": coins,
             "tippingContext": {"transactionId": transactionId},
         }
 
-        if blogId != None: url = f"{api}/g/s/blog/{blogId}/tipping"
-        if chatId != None: url = f"{api}/g/s/chat/thread/{chatId}/tipping"
-        if objectId != None:
+        if blogId is not None:
+            url = f"{api}/g/s/blog/{blogId}/tipping"
+        if chatId is not None:
+            url = f"{api}/g/s/chat/thread/{chatId}/tipping"
+        if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
             url = f"{api}/g/s/tipping"
 
-        if url is None: raise exceptions.SpecifyType
+        if url is None:
+            raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.status_code
 
     def follow(self, userId: Union[str, list]):
         """
         Follow an User or Multiple Users.
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         if isinstance(userId, str):
             response = self.session.post(f"{api}/g/s/user-profile/{userId}/member")
 
         elif isinstance(userId, list):
             data = {"targetUidList": userId}
-            
             response = self.session.post(f"{api}/g/s/user-profile/{self.profile.userId}/joined", json=data)
 
         else: raise exceptions.WrongType
 
         return response.status_code
 
     def unfollow(self, userId: str):
@@ -1157,45 +1282,45 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.delete(f"{api}/g/s/user-profile/{userId}/member/{self.profile.userId}")
         return response.status_code
 
     def block(self, userId: str):
         """
         Block an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.post(f"{api}/g/s/block/{userId}")
         return response.status_code
 
     def unblock(self, userId: str):
         """
         Unblock an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.delete(f"{api}/g/s/block/{userId}")
         return response.status_code
 
     def join_community(self, comId: int, invitationId: str = None):
         """
         Join a Community.
@@ -1203,18 +1328,19 @@
         **Parameters**
             - **comId** : ID of the Community.
             - **invitationId** : ID of the Invitation Code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        data = dict()
-        if invitationId: data["invitationId"] = invitationId
+        data = {}
+        if invitationId:
+            data["invitationId"] = invitationId
 
         response = self.session.post(f"{api}/x{comId}/s/community/join", json=data)
         return response.status_code
 
     def request_join_community(self, comId: int, message: str = None):
         """
         Request to join a Community.
@@ -1222,15 +1348,15 @@
         **Parameters**
             - **comId** : ID of the Community.
             - **message** : Message to be sent.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {"message": message}
 
         response = self.session.post(f"{api}/x{comId}/s/community/membership-request", jaon=data)
         return response.status_code
 
     def leave_community(self, comId: int):
@@ -1239,15 +1365,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.post(f"{api}/x{comId}/s/community/leave")
         return response.status_code
 
     def flag_community(self, comId: int, reason: str, flagType: int, isGuest: bool = False):
         """
         Flag a Community.
@@ -1256,29 +1382,32 @@
             - **comId** : ID of the Community.
             - **reason** : Reason of the Flag.
             - **flagType** : Type of Flag.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if reason is None: raise exceptions.ReasonNeeded
-        if flagType is None: raise exceptions.FlagTypeNeeded
+        if reason is None:
+            raise exceptions.ReasonNeeded
+        if flagType is None:
+            raise exceptions.FlagTypeNeeded
 
         data = {
             "objectId": comId,
             "objectType": 16,
             "flagType": flagType,
             "message": reason,
         }
 
-        if isGuest: flg = "g-flag"
-        else: flg = "flag"
-        
+        if isGuest:
+            flg = "g-flag"
+        else:
+            flg = "flag"
         response = self.session.post(f"{api}/x{comId}/s/{flg}", json=data)
         return response.status_code
 
     def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, backgroundColor: str = None, backgroundImage: str = None, defaultBubbleId: str = None):
         """
         Edit account's Profile.
 
@@ -1289,124 +1418,129 @@
             - **backgroundImage** : Url of the Background Picture of the Profile.
             - **backgroundColor** : Hexadecimal Background Color of the Profile.
             - **defaultBubbleId** : Chat bubble ID.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "address": None,
             "latitude": 0,
             "longitude": 0,
             "mediaList": None,
             "eventSource": "UserProfileView",
         }
 
-        if nickname: data["nickname"] = nickname
-        if icon: data["icon"] = upload_media(self, icon, "image")
-        if content: data["content"] = content
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
-        if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
-        if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+        if nickname:
+            data["nickname"] = nickname
+        if icon:
+            data["icon"] = upload_media(self, icon, "image")
+        if content:
+            data["content"] = content
+        if backgroundColor:
+            data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if backgroundImage:
+            data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
+        if defaultBubbleId:
+            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
 
         response = self.session.post(f"{api}/g/s/user-profile/{self.profile.userId}", json=data)
         return response.status_code
 
     def set_amino_id(self, aminoId: str):
         """
         Edit account's Amino ID.
 
         **Parameters**
             - **aminoId** : Amino ID of the Account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {"aminoId": aminoId}
 
         response = self.session.post(f"{api}/g/s/account/change-amino-id", json=data)
         return response.status_code
 
     def get_linked_communities(self, userId: str):
         """
         Get a List of Linked Communities of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <AminoLightPy.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/user-profile/{userId}/linked-community")
         return objects.CommunityList(response.json()["linkedCommunityList"]).CommunityList
 
     def get_unlinked_communities(self, userId: str):
         """
         Get a List of Unlinked Communities of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <AminoLightPy.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/user-profile/{userId}/linked-community")
         return objects.CommunityList(response.json()["unlinkedCommunityList"]).CommunityList
 
     def reorder_linked_communities(self, comIds: list):
         """
         Reorder List of Linked Communities.
 
         **Parameters**
             - **comIds** : IDS of the Communities.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {"ndcIds": comIds}
-
         response = self.session.post(f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/reorder", json=data)
         return response.status_code
 
     def add_linked_community(self, comId: int):
         """
         Add a Linked Community on your profile.
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.post(f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/{comId}")
         return response.status_code
 
     def remove_linked_community(self, comId: int):
         """
         Remove a Linked Community on your profile.
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.delete(f"{api}/g/s/user-profile/{self.profile.userId}/linked-community/{comId}")
         return response.status_code
 
     def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None):
         """
         Comment on a User's Wall, Blog or Wiki.
@@ -1417,39 +1551,38 @@
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
             - **replyTo** : ID of the Comment to Reply to.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if message is None: raise exceptions.MessageNeeded
+        if message is None:
+            raise exceptions.MessageNeeded
 
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
         }
 
-        if replyTo: data["respondTo"] = replyTo
+        if replyTo:
+            data["respondTo"] = replyTo
 
         if userId:
             data["eventSource"] = "UserProfileView"
-            
             url = f"{api}/g/s/user-profile/{userId}/g-comment"
 
         elif blogId:
             data["eventSource"] = "PostDetailView"
-            
             url = f"{api}/g/s/blog/{blogId}/g-comment"
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
-            
             url = f"{api}/g/s/item/{wikiId}/g-comment"
 
         else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.status_code
 
@@ -1462,20 +1595,24 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if userId: url = f"{api}/g/s/user-profile/{userId}/g-comment/{commentId}"
-        elif blogId: url = f"{api}/g/s/blog/{blogId}/g-comment/{commentId}"
-        elif wikiId: url = f"{api}/g/s/item/{wikiId}/g-comment/{commentId}"
-        else: raise exceptions.SpecifyType
+        if userId:
+            url = f"{api}/g/s/user-profile/{userId}/g-comment/{commentId}"
+        elif blogId:
+            url = f"{api}/g/s/blog/{blogId}/g-comment/{commentId}"
+        elif wikiId:
+            url = f"{api}/g/s/item/{wikiId}/g-comment/{commentId}"
+        else:
+            raise exceptions.SpecifyType
 
         response = self.session.delete(url)
         return response.status_code
 
     def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None):
         """
         Like a Blog, Multiple Blogs or a Wiki.
@@ -1483,37 +1620,33 @@
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "value": 4,
         }
 
         if blogId:
             if isinstance(blogId, str):
                 data["eventSource"] = "UserProfileView"
-                
                 url = f"{api}/g/s/blog/{blogId}/g-vote?cv=1.2"
 
             elif isinstance(blogId, list):
                 data["targetIdList"] = blogId
-                
                 url = f"{api}/g/s/feed/g-vote"
 
             else: raise exceptions.WrongType(type(blogId))
 
-
         elif wikiId:
             data["eventSource"] = "PostDetailView"
-            
             url = f"{api}/g/s/item/{wikiId}/g-vote?cv=1.2"
 
         else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.status_code
 
@@ -1524,20 +1657,22 @@
         **Parameters**
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if blogId: url = f"{api}/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView"
-        elif wikiId: url = f"{api}/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView"
-        else: raise exceptions.SpecifyType
-        
+        if blogId:
+            url = f"{api}/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView"
+        elif wikiId:
+            url = f"{api}/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView"
+        else:
+            raise exceptions.SpecifyType
         response = self.session.delete(url)
         return response.status_code
 
     def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
         """
         Like a Comment on a User's Wall, Blog or Wiki.
 
@@ -1546,33 +1681,30 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "value": 4,
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
-            
             url = f"{api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1"
 
         elif blogId:
             data["eventSource"] = "PostDetailView"
-            
             url = f"{api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?cv=1.2&value=1"
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
-            
             url = f"{api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1"
 
         else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.status_code
 
@@ -1585,35 +1717,39 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if userId: url = f"{api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView"
-        elif blogId: url = f"{api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
-        elif wikiId: url = f"{api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
-        else: raise exceptions.SpecifyType
+        if userId:
+            url = f"{api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView"
+        elif blogId:
+            url = f"{api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
+        elif wikiId:
+            url = f"{api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
+        else:
+            raise exceptions.SpecifyType
 
         response = self.session.delete(url)
         return response.status_code
 
     def get_membership_info(self):
         """
         Get Information about your Amino+ Membership.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
-            - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
+            - **Success** : :meth:`Membership Object <AminoLightPy.lib.util.objects.Membership>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/membership?force=true")
         return objects.Membership(response.json()).Membership
 
     def get_ta_announcements(self, language: str = "en", start: int = 0, size: int = 25):
         """
         Get the list of Team Amino's Announcement Blogs.
@@ -1621,136 +1757,143 @@
         **Parameters**
             - **language** : Language of the Blogs.
                 - ``en``, ``es``, ``pt``, ``ar``, ``ru``, ``fr``, ``de``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
+            - **Success** : :meth:`Blogs List <AminoLightPy.lib.util.objects.BlogList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        if language not in self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
-        response = self.session.get(f"{api}/g/s/announcement?language={language}&start={start}&size={size}")
+        if language not in self.get_supported_languages():
+            raise exceptions.UnsupportedLanguage(language)
+        params = {
+            "language": language,
+            "start": start,
+            "size": size
+        }
+        response = self.session.get(f"{api}/g/s/announcement", params=params)
         return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_wallet_info(self):
         """
         Get Information about the account's Wallet.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+            - **Success** : :meth:`Wallet Object <AminoLightPy.lib.util.objects.WalletInfo>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/wallet")
         return objects.WalletInfo(response.json()["wallet"]).WalletInfo
 
     def get_wallet_history(self, start: int = 0, size: int = 25):
         """
         Get the Wallet's History Information.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+            - **Success** : :meth:`Wallet Object <AminoLightPy.lib.util.objects.WalletInfo>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/wallet/coin/history?start={start}&size={size}")
         return objects.WalletHistory(response.json()["coinHistoryList"]).WalletHistory
 
     def get_from_deviceid(self, deviceId: str):
         """
         Get the User ID from an Device ID.
 
         **Parameters**
             - **deviceID** : ID of the Device.
 
         **Returns**
-            - **Success** : :meth:`User ID <amino.lib.util.objects.UserProfile.userId>`
+            - **Success** : :meth:`User ID <AminoLightPy.lib.util.objects.UserProfile.userId>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/auid?deviceId={deviceId}")
         return response.json()["auid"]
 
     def get_from_code(self, code: str):
         """
         Get the Object Information from the Amino URL Code.
 
         **Parameters**
             - **code** : Code from the Amino URL.
                 - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
 
         **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+            - **Success** : :meth:`From Code Object <AminoLightPy.lib.util.objects.FromCode>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/link-resolution?q={code}")
         return objects.FromCode(response.json()["linkInfoV2"]).FromCode
 
     def get_from_id(self, objectId: str, objectType: int, comId: int = None):
         """
         Get the Object Information from the Object ID and Type.
 
         **Parameters**
             - **objectID** : ID of the Object. User ID, Blog ID, etc.
             - **objectType** : Type of the Object.
             - *comId* : ID of the Community. Use if the Object is in a Community.
 
         **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+            - **Success** : :meth:`From Code Object <AminoLightPy.lib.util.objects.FromCode>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "objectId": objectId,
             "targetCode": 1,
             "objectType": objectType,
         }
-        
-        if comId: url = f"{api}/g/s-x{comId}/link-resolution"
-        else: url = f"{api}/g/s/link-resolution"
+        if comId:
+            url = f"{api}/g/s-x{comId}/link-resolution"
+        else:
+            url = f"{api}/g/s/link-resolution"
 
         response = self.session.post(url, json=data)
         return objects.FromCode(response.json()["linkInfoV2"]).FromCode
 
     def get_supported_languages(self):
         """
         Get the List of Supported Languages by Amino.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`List of Supported Languages <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/community-collection/supported-languages?start=0&size=100")
         return response.json()["supportedLanguages"]
 
     def claim_new_user_coupon(self):
         """
         Claim the New User Coupon available when a new account is created.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.post(f"{api}/g/s/coupon/new-user-coupon/claim")
         return response.status_code
 
     def get_subscriptions(self, start: int = 0, size: int = 25):
         """
         Get Information about the account's Subscriptions.
@@ -1758,59 +1901,91 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/store/subscription?objectType=122&start={start}&size={size}")
         return response.json()["storeSubscriptionItemList"]
 
     def get_all_users(self, start: int = 0, size: int = 25):
         """
         Get list of users of Amino.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
+            - **Success** : :meth:`User Profile Count List Object <AminoLightPy.lib.util.objects.UserProfileCountList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/user-profile?type=recent&start={start}&size={size}")
         return objects.UserProfileCountList(response.json()).UserProfileCountList
 
     def accept_host(self, chatId: str, requestId: str):
+        """
+        Accepts a host request for a chat.
+
+        **Parameters**
+            - **chatId** (str): ID of the chat.
+            - **requestId** (str): ID of the host request.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept")
         return response.status_code
 
     def accept_organizer(self, chatId: str, requestId: str):
+        """
+        Accepts a host request for a chat.
+
+        **Parameters**
+            - **chatId** (str): ID of the chat.
+            - **requestId** (str): ID of the host request.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         self.accept_host(chatId, requestId)
 
     # Contributed by 'https://github.com/LynxN1'
     def link_identify(self, code: str):
+        """
+        Identifies a community link.
+
+        **Parameters**
+            - **code** (str): The code of the community link.
+
+        **Returns**
+            - **Success** : A JSON object with the community link information.
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         response = self.session.get(f"{api}/g/s/community/link-identify?q=http%3A%2F%2Faminoapps.com%2Finvite%2F{code}")
         return response.json()
 
     def invite_to_vc(self, chatId: str, userId: str):
         """
         Invite a User to a Voice Chat
 
         **Parameters**
             - **chatId** - ID of the Chat
             - **userId** - ID of the User
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         data = {
             "uid": userId
         }
 
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/vvchat-presenter/invite", json=data)
@@ -1823,25 +1998,36 @@
         **Parameters**
             - **level** - Level of the ads.
                 - ``1``, ``2``
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         data = {
             "adsLevel": level,
         }
 
         response = self.session.post(f"{api}/g/s/wallet/ads/config", json=data)
         return response.status_code
 
     def purchase(self, objectId: str, isAutoRenew: bool = False):
+        """
+        Makes a purchase in the store.
+
+        **Parameters**
+            - **objectId** (str): ID of the object to be purchased.
+            - *isAutoRenew* (bool, optional): Whether the purchase should be auto-renewed. Defaults to False.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         data = {
             "objectId": objectId,
             "objectType": 114,
             "v": 1,
             "paymentContext":
             {
                 "discountStatus": 0,
@@ -1856,27 +2042,34 @@
         """
         Get public communites
 
         **Parameters**
             - **language** - Set up language
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <AminoLightPy.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
+        params = {
+            "language": language,
+            "type": "web-explore",
+            "categoryKey": "recommendation",
+            "size": size,
+            "pagingType": "t"
+        }
 
-        response = self.session.get(f"{api}/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t")
+        response = self.session.get(f"{api}/g/s/topic/0/feed/community", params=params)
         return objects.CommunityList(response.json()["communityList"]).CommunityList
 
 
     def get_blockers(self) -> list[str]:
         """
         Get ids of user ho block you.
 
         **Returns**
             - **Success** : :meth:`List <str>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/g/s/block/full-list")
-        return response.json()["blockerUidList"]
+        return response.json()["blockerUidList"]
```

### Comparing `amino.light.py-0.1.1/AminoLightPy/constants.py` & `amino.light.py-0.1.2/AminoLightPy/constants.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.1/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.2/AminoLightPy/lib/util/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,881 +1,881 @@
-from json import loads
+from json import loads, JSONDecodeError
 
 class UnsupportedService(Exception):
     """
     - **API Code** : 100
     - **API Message** : Unsupported service. Your client may be out of date. Please update it to the latest version.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class FileTooLarge(Exception):
     """
     - **API Code** : 102
     - **API Message** : ``Unknown Message``
     - **API String** : API_STD_ERR_ENTITY_TOO_LARGE_RAW
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidRequest(Exception):
     """
     - **API Code** : 103, 104
     - **API Message** : Invalid Request. Please update to the latest version. If the problem continues, please contact us.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidSession(Exception):
     """
     - **API Code** : 105
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AccessDenied(Exception):
     """
     - **API Code** : 106
     - **API Message** : Access denied.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UnexistentData(Exception):
     """
     - **API Code** : 107
     - **API Message** : The requested data does not exist.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ActionNotAllowed(Exception):
     """
     - **API Code** : 110
     - **API Message** : Action not allowed.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ServiceUnderMaintenance(Exception):
     """
     - **API Code** : 111
     - **API Message** : Sorry, this service is under maintenance. Please check back later.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class MessageNeeded(Exception):
     """
     - **API Code** : 113
     - **API Message** : Be more specific, please.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidAccountOrPassword(Exception):
     """
     - **API Code** : 200
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AccountDisabled(Exception):
     """
     - **API Code** : 210
     - **API Message** : This account is disabled.
     - **API String** : AUTH_DISABLED_ACCOUNT
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidEmail(Exception):
     """
     - **API Code** : 213
     - **API Message** : Invalid email address.
     - **API String** : API_ERR_EMAIL
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidPassword(Exception):
     """
     - **API Code** : 214
     - **API Message** : Invalid password. Password must be 6 characters or more and contain no spaces.
     - **API String** : API_ERR_PASSWORD
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class EmailAlreadyTaken(Exception):
     """
     - **API Code** : 215
     - **API Message** : Hey this email ``X`` has been registered already. You can try to log in with the email or edit the email.
     - **API String** : API_ERR_EMAIL_TAKEN
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UnsupportedEmail(Exception):
     """
     - **API Code** : 215
     - **API Message** : This email address is not supported.
     - **API String** : API_ERR_EMAIL_TAKEN
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AccountDoesntExist(Exception):
     """
     - **API Code** : 216
     - **API Message** : ``Unknown Message``
     - **API String** : AUTH_ACCOUNT_NOT_EXISTS
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidDevice(Exception):
     """
     - **API Code** : 218
     - **API Message** : Error! Your device is currently not supported, or the app is out of date. Please update to the latest version.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AccountLimitReached(Exception):
     """
     - **API Code** : 219
     - **API Message** : A maximum of 3 accounts can be created from this device. If you forget your password, please reset it.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class TooManyRequests(Exception):
     """
     - **API Code** : 219
     - **API Message** : Too many requests. Try again later.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CantFollowYourself(Exception):
     """
     - **API Code** : 221
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UserUnavailable(Exception):
     """
     - **API Code** : 225
     - **API Message** : This user is unavailable.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class YouAreBanned(Exception):
     """
     - **API Code** : 229
     - **API Message** : You are banned.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UserNotMemberOfCommunity(Exception):
     """
     - **API Code** : 230
     - **API Message** : You have to join this Community first.
     - **API String** : API_ERR_USER_NOT_IN_COMMUNITY
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class RequestRejected(Exception):
     """
     - **API Code** : 235
     - **API Message** : Request rejected. You have been temporarily muted (read only mode) because you have received a strike. To learn more, please check the Help Center.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ActivateAccount(Exception):
     """
     - **API Code** : 238
     - **API Message** : Please activate your account first. Check your email, including your spam folder.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CantLeaveCommunity(Exception):
     """
     - **API Code** : 239
     - **API Message** : Sorry, you can not do this before transferring your Agent status to another member.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ReachedTitleLength(Exception):
     """
     - **API Code** : 240
     - **API Message** : Sorry, the max length of member's title is limited to 20.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AccountDeleted(Exception):
     """
     - **API Code** : 246
     - **API Message** : ``Unknown Message``
     - **API String** : AUTH_RECOVERABLE_DELETED_ACCOUNT
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_EMAIL_NO_PASSWORD(Exception):
     """
     - **API Code** : 251
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_EMAIL_NO_PASSWORD
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_COMMUNITY_USER_CREATED_COMMUNITIES_VERIFY(Exception):
     """
     - **API Code** : 257
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_COMMUNITY_USER_CREATED_COMMUNITIES_VERIFY
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ReachedMaxTitles(Exception):
     """
     - **API Code** : 262
     - **API Message** : You can only add up to 20 Titles. Please choose the most relevant ones.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class VerificationRequired(Exception):
     """
     - **API Code** : 270
     - **API Message** : Verification Required.
     - **API String** : API_ERR_NEED_TWO_FACTOR_AUTHENTICATION
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_INVALID_AUTH_NEW_DEVICE_LINK(Exception):
     """
     - **API Code** : 271
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_INVALID_AUTH_NEW_DEVICE_LINK
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommandCooldown(Exception):
     """
     - **API Code** : 291
     - **API Message** : Whoa there! You've done too much too quickly. Take a break and try again later.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UserBannedByTeamAmino(Exception):
     """
     - **API Code** : 293
     - **API Message** : Sorry, this user has been banned by Team Amino.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class BadImage(Exception):
     """
     - **API Code** : 300
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidThemepack(Exception):
     """
     - **API Code** : 313
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidVoiceNote(Exception):
     """
     - **API Code** : 314
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class RequestedNoLongerExists(Exception):
     """
     - **API Code** : 500, 700, 1600
     - **API Message** : Sorry, the requested data no longer exists. Try refreshing the view.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class PageRepostedTooRecently(Exception):
     """
     - **API Code** : 503
     - **API Message** : Sorry, you have reported this page too recently.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InsufficientLevel(Exception):
     """
     - **API Code** : 551
     - **API Message** : This post type is restricted to members with a level ``X`` ranking and above.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class WallCommentingDisabled(Exception):
     """
     - **API Code** : 702
     - **API Message** : This member has disabled commenting on their wall.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommunityNoLongerExists(Exception):
     """
     - **API Code** : 801
     - **API Message** : This Community no longer exists.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidCodeOrLink(Exception):
     """
     - **API Code** : 802
     - **API Message** : Sorry, this code or link is invalid.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommunityNameAlreadyTaken(Exception):
     """
     - **API Code** : 805
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommunityCreateLimitReached(Exception):
     """
     - **API Code** : 806
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_COMMUNITY_USER_CREATED_COMMUNITIES_EXCEED_QUOTA
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommunityDisabled(Exception):
     """
     - **API Code** : 814
     - **API Message** : This Community is disabled.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommunityDeleted(Exception):
     """
     - **API Code** : 833
     - **API Message** : This Community has been deleted.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class DuplicatePollOption(Exception):
     """
     - **API Code** : 1501
     - **API Message** : Sorry, you have duplicate poll options.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ReachedMaxPollOptions(Exception):
     """
     - **API Code** : 1507
     - **API Message** : Sorry, you can only join or add up to 5 of your items per poll.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class TooManyChats(Exception):
     """
     - **API Code** : 1602
     - **API Message** : Sorry, you can only have up to 1000 chat sessions.
     - **API String** : ``Unknown String``
     """
 
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ChatFull(Exception):
     """
     - **API Code** : 1605
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class TooManyInviteUsers(Exception):
     """
     - **API Code** : 1606
     - **API Message** : Sorry, you can only invite up to 999 people.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ChatInvitesDisabled(Exception):
     """
     - **API Code** : 1611
     - **API Message** : This user has disabled chat invite requests.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class RemovedFromChat(Exception):
     """
     - **API Code** : 1612
     - **API Message** : You've been removed from this chatroom.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UserNotJoined(Exception):
     """
     - **API Code** : 1613
     - **API Message** : Sorry, this user has not joined.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_CHAT_VVCHAT_NO_MORE_REPUTATIONS(Exception):
     """
     - **API Code** : 1627
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_CHAT_VVCHAT_NO_MORE_REPUTATIONS
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class MemberKickedByOrganizer(Exception):
     """
     - **API Code** : 1637
     - **API Message** : This member was previously kicked by the organizer and cannot be reinvited.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class LevelFiveRequiredToEnableProps(Exception):
     """
     - **API Code** : 1661
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ChatViewOnly(Exception):
     """
     - **API Code** : 1663
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ChatMessageTooBig(Exception):
     """
     - **API Code** : 1664
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_CHAT_MESSAGE_CONTENT_TOO_LONG
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InviteCodeNotFound(Exception):
     """
     - **API Code** : 1900
     - **API Message** : Sorry, the requested data no longer exists. Try refreshing the view.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AlreadyRequestedJoinCommunity(Exception):
     """
     - **API Code** : 2001
     - **API Message** : Sorry, you have already submitted a membership request.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_PUSH_SERVER_LIMITATION_APART(Exception):
     """
     - **API Code** : 2501
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_PUSH_SERVER_LIMITATION_APART
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_PUSH_SERVER_LIMITATION_COUNT(Exception):
     """
     - **API Code** : 2502
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_PUSH_SERVER_LIMITATION_COUNT
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_PUSH_SERVER_LINK_NOT_IN_COMMUNITY(Exception):
     """
     - **API Code** : 2503
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_PUSH_SERVER_LINK_NOT_IN_COMMUNITY
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class API_ERR_PUSH_SERVER_LIMITATION_TIME(Exception):
     """
     - **API Code** : 2504
     - **API Message** : ``Unknown Message``
     - **API String** : API_ERR_PUSH_SERVER_LIMITATION_TIME
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AlreadyCheckedIn(Exception):
     """
     - **API Code** : 2601
     - **API Message** : Sorry, you can't check in any more.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AlreadyUsedMonthlyRepair(Exception):
     """
     - **API Code** : 2611
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AccountAlreadyRestored(Exception):
     """
     - **API Code** : 2800
     - **API Message** : Account already restored.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class IncorrectVerificationCode(Exception):
     """
     - **API Code** : 3102
     - **API Message** : Incorrect verification code.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class NotOwnerOfChatBubble(Exception):
     """
     - **API Code** : 3905
     - **API Message** : You are not the owner of this chat bubble.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class NotEnoughCoins(Exception):
     """
     - **API Code** : 4300
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AlreadyPlayedLottery(Exception):
     """
     - **API Code** : 4400
     - **API Message** : You have played the maximum number of lucky draws.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CannotSendCoins(Exception):
     """
     - **API Code** : 4500, 4501
     - **API Message** : ``Unknown Message``
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AminoIDAlreadyChanged(Exception):
     """
     - **API Code** : 6001
     - **API Message** : Amino ID cannot be changed after you set it.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidAminoID(Exception):
     """
     - **API Code** : 6002
     - **API Message** : Invalid Amino ID
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class InvalidName(Exception):
     """
     - **API Code** : 99001
     - **API Message** : Sorry, the name is invalid.
     - **API String** : ``Unknown String``
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class SpecifyType(Exception):
     """
     Raised when you need to specify the output of the command.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class WrongType(Exception):
     """
     Raised when you attribute the function the wrong type.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UnknownResponse(Exception):
     """
     Raised when an error occurs but the reason is unknown.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class NotLoggedIn(Exception):
     """
     Raised when you try to make an action but you aren't logged in.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class NoCommunity(Exception):
     """
     Raised when you try to make an action but no community was selected.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommunityNotFound(Exception):
     """
     Raised when you search for a community but nothing is found.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class NoChatThread(Exception):
     """
     Raised when you try to make an action but no chat was selected.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ChatRequestsBlocked(Exception):
     """
     Raised when you try to make an action but the end user has chat requests blocked.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class NoImageSource(Exception):
     """
     Raised when you try to make an action but no image source was selected.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CannotFetchImage(Exception):
     """
     Raised when an image cannot be fetched.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class FailedLogin(Exception):
     """
     Raised when you try to login but it fails.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class AgeTooLow(Exception):
     """
     Raised when you try to configure an account but the age is too low. Minimum is 13.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UnsupportedLanguage(Exception):
     """
     Raised when you try to use a language that isn't supported or exists.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class CommunityNeeded(Exception):
     """
     Raised when you try to execute an command but a Community needs to be specified.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class FlagTypeNeeded(Exception):
     """
     Raised when you try to flag a community, blog or user but a Flag Type needs to be specified.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class ReasonNeeded(Exception):
     """
     Raised when you try to execute an command but a Reason needs to be specified.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 
 class TransferRequestNeeded(Exception):
     """
     Raised when you need to transfer host to complete the action.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class LibraryUpdateAvailable(Exception):
     """
     Raised when a new library update is available.
     """
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UserHasBeenDeleted(Exception):
     """
     - **API Code** : 245
     - **API Message** : Sorry, this user has been deleted.
     - **API String** : ``Unknown String``
     """
 
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class IpTemporaryBan(Exception):
     """
     - **API Code** : 403
     - **API Message** : 403 Forbidden.
     - **API String** : ``Unknown String``
     """
 
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class FailedSubscribeFanClub(Exception):
     """
     - **API Code** : 4805
     - **API Message** : Failed to subscribe to this fan club.
     - **API String** : ``Unknown String``
     """
 
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 class UnknownError(Exception):
-    def __init__(*args, **kwargs):
-        Exception.__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 def CheckException(data):
     try:
         data = loads(data)
         try:
             api_code = data["api:statuscode"]
-        except:
-            raise UnknownError(data)
-    except:
+        except KeyError as e:
+            raise UnknownError(data) from e
+    except JSONDecodeError:
         api_code = 403
 
     if api_code == 100: raise UnsupportedService(data)
     elif api_code == 102: raise FileTooLarge(data)
     elif api_code == 103 or api_code == 104: raise InvalidRequest(data)
     elif api_code == 105: raise InvalidSession(data)
     elif api_code == 106: raise AccessDenied(data)
```

### Comparing `amino.light.py-0.1.1/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.2/AminoLightPy/lib/util/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 from base64 import b64decode, b64encode
 
 PREFIX = b'\x19'
 SIG_KEY = b'\xdf\xa5\xed\x19-\xdan\x88\xa1/\xe1!0\xdcb\x06\xb1%\x1eD'
 DEVICE_KEY = b"\xe70\x9e\xcc\tS\xc6\xfa`\x00['e\xf9\x9d\xbb\xc9e\xc8\xe9"
 
 def gen_deviceId(data: bytes = None) -> str:
-    if isinstance(data, str): data = bytes(data, 'utf-8')
+    if isinstance(data, str):
+        data = bytes(data, 'utf-8')
     identifier = PREFIX + (data or urandom(20))
     mac = new(DEVICE_KEY, identifier, sha1)
     return f"{identifier.hex()}{mac.hexdigest()}".upper()
 
 def signature(data: Union[str, bytes]) -> str:
     data = data if isinstance(data, bytes) else data.encode("utf-8")
     return b64encode(PREFIX + new(SIG_KEY, data, sha1).digest()).decode("utf-8")
 
 def update_deviceId(device: str) -> str:
     return gen_deviceId(bytes.fromhex(device[2:42]))
 
 def self_deviceId(email: str) -> str:
-    hash = sha1(email.encode()).digest()
-    return gen_deviceId(hash)
+    return gen_deviceId(sha1(email.encode()).digest())
 
 def decode_sid(sid: str) -> dict:
     sid = sid.replace("-", "+").replace("_", "/")
     sid += "=" * (-len(sid) % 4)
     decoded_bytes = b64decode(sid.encode())
     return loads(decoded_bytes[1:-20].decode())
 
-def sid_to_uid(SID: str) -> str: return decode_sid(SID)["2"]
+def sid_to_uid(SID: str) -> str:
+    return decode_sid(SID)["2"]
 
-def sid_to_ip_address(SID: str) -> str: return decode_sid(SID)["4"]
+def sid_to_ip_address(SID: str) -> str:
+    return decode_sid(SID)["4"]
```

### Comparing `amino.light.py-0.1.1/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.1.2/AminoLightPy/lib/util/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=invalid-name
 # You don't even know how long this shit took...
 # F*ck you Sand for making me do this.
 
 from typing import List, Optional, Dict, TypeVar
 
 class UserProfile:
     __slots__ = (
@@ -24,15 +25,15 @@
         "warningCount", "session"
     )
 
     def __init__(self, data: Dict):
         if data is None:
             for attr in self.__slots__:
                 setattr(self, attr, None)
-        
+
             return
 
         self.json: Optional[Dict] = data
 
         self.fanClub = FanClubList(data.get("fanClubList", [])).FanClubList
 
         self.accountMembershipStatus: Optional[int] = data.get("accountMembershipStatus")
@@ -112,16 +113,14 @@
         self.staffInfo: Optional[Dict] = data.get("adminInfo", {})
         self.globalStrikeCount: Optional[int] = self.staffInfo.get("globalStrikeCount")
         self.lastStrikeTime: Optional[int] = self.staffInfo.get("lastStrikeTime")
         self.lastWarningTime: Optional[int] = self.staffInfo.get("lastWarningTime")
         self.strikeCount: Optional[int] = self.staffInfo.get("strikeCount")
         self.warningCount: Optional[int] = self.staffInfo.get("warningCount")
 
-
-        
         self.session = None
 
     @property
     def UserProfile(self):
 
         return self
 
@@ -454,15 +453,15 @@
         "themeLeftSidePanelColor", "customList"
     )
 
     def __init__(self, data: Dict):
         if data is None:
             for attr in self.__slots__:
                 setattr(self, attr, None)
-        
+
             return
 
         self.json = data
 
         self.agent: UserProfile = UserProfile(data.get("agent", [])).UserProfile
 
         try: self.rankingTable: RankingTableList = RankingTableList(data["advancedSettings"]["rankingTable"]).RankingTableList
@@ -541,15 +540,14 @@
         self.json = data
         _communtyObjects = tuple(Community(x).Community for x in data)
 
         set_attributes(self, _communtyObjects)
 
     @property
     def CommunityList(self):
-    
         return self
 
 class CommentList:
     def __init__(self, data):
         self.json = data
         self.author = UserProfileList(tuple(y.get("author") for y in data)).UserProfileList
         self.votesSum = tuple(x.get("votesSum") for x in data)
@@ -622,17 +620,17 @@
         "json", "profile", "userProfileCount"
     )
 
     def __init__(self, data):
         if data is None:
             for attr in self.__slots__:
                 setattr(self, attr, None)
-        
+
             return
-            
+
         self.json = data
 
         self.profile: UserProfileList = UserProfileList(data.get("userProfileList")).UserProfileList
 
         self.userProfileCount = data.get("userProfileCount")
 
     @property
@@ -867,15 +865,15 @@
         "vvChatJoinType", "disabledTime", "tippingPermStatus", "screeningRoomHostId", "screeningRoomPermission",
         "organizerTransferCreatedTime", "organizerTransferId"
     )
     def __init__(self, data):
         if data is None:
             for attr in self.__slots__:
                 setattr(self, attr, None)
-        
+
             return
 
         self.json = data
 
         self.author: UserProfile = UserProfile(data.get("author")).UserProfile
         self.membersSummary: UserProfileList = UserProfileList(data.get("membersSummary")).UserProfileList
 
@@ -1049,17 +1047,17 @@
         "mediumIconV2", "extensions", "usedCount", "createdTime"
     )
 
     def __init__(self, data):
         if data is None:
             for attr in self.__slots__:
                 setattr(self, attr, None)
-        
+
             return
-            
+
         self.json = data
 
         self.collection: StickerCollection = StickerCollection(data.get("stickerCollectionSummary")).StickerCollection
 
         self.status: Optional[str] = data.get("status")
         self.icon: Optional[str] = data.get("icon")
         self.iconV2: Optional[str] = data.get("iconV2")
@@ -1103,15 +1101,15 @@
         self.bannerUrl = data.get("bannerUrl")
         self.smallIcon = data.get("smallIcon")
         self.stickersCount = data.get("stickersCount")
         self.usedCount = data.get("usedCount")
         self.icon = data.get("icon")
         self.title = data.get("name")
         self.collectionId = data.get("collectionId")
-        
+
         self.isActivated = data.get("isActivated")
         self.ownershipStatus = data.get("ownershipStatus")
         self.isNew = data.get("isNew")
         self.availableComIds = data.get("availableNdcIds")
         self.description = data.get("description")
 
         #extensions
@@ -1439,15 +1437,15 @@
             self.objectUrl.append(x.get("objectUrl"))
 
         return self
 
 class LotteryLog:
     def __init__(self, data):
         self.json = data
-        
+
         self.awardValue = data.get("awardValue")
         self.parentId = data.get("parentId")
         self.parentType = data.get("parentType")
         self.objectId = data.get("objectId")
         self.objectType = data.get("objectType")
         self.createdTime = data.get("createdTime")
         self.awardType = data.get("awardType")
@@ -2352,8 +2350,8 @@
 class MediaObject(List[List[TypeVar('T')]]):
     pass
 
 def set_attributes(instance, _ListObjects):
     if _ListObjects:
         attributes = tuple(attr for attr in dir(_ListObjects[0]) if not attr.startswith('__') and not callable(getattr(_ListObjects[0], attr)) and attr != _ListObjects[0].__class__.__name__)
         for attr in attributes:
-            setattr(instance, attr, tuple(getattr(user, attr, None) for user in _ListObjects))
+            setattr(instance, attr, tuple(getattr(user, attr, None) for user in _ListObjects))
```

### Comparing `amino.light.py-0.1.1/AminoLightPy/socket.py` & `amino.light.py-0.1.2/AminoLightPy/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=invalid-name
+
 from json import loads, dumps
 from time import time, sleep
 from threading import Thread
 from websocket import WebSocketApp
 
 from .lib.util.objects import Event
 from .lib.util.helpers import gen_deviceId, signature
@@ -88,17 +90,16 @@
 
     def debug_print(self, message):
         if self.debug:
             print(message)
 
 
 class SocketRequests:
-    def __init__(self, socket: SocketHandler) -> None:
+    def __init__(self) -> None:
         self.active_live_chats = set()
-        self.socket = socket
 
     def join_voice_chat(self, comId: int, chatId: str, joinType: int = 1):
         """
         Joins a Voice Chat
         **Parameters**
             - **comId** : ID of the Community
             - **chatId** : ID of the Chat
@@ -111,15 +112,15 @@
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
             },
             "t": 112
         }
         data = dumps(data)
-        self.soket.send(data)
+        self.send(data)
 
     def join_video_chat(self, comId: int, chatId: str, joinType: int = 1):
         """
         Joins a Video Chat
         **Parameters**
             - **comId** : ID of the Community
             - **chatId** : ID of the Chat
@@ -133,28 +134,28 @@
                 "threadId": chatId,
                 "joinRole": joinType,
                 "channelType": 5,
             },
             "t": 108
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
     def join_video_chat_as_viewer(self, comId: int, chatId: str):
         data = {
             "o":
                 {
                     "ndcId": int(comId),
                     "threadId": chatId,
                     "joinRole": 2,
                 },
             "t": 112
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
 
     # Fixed by vedansh#4039
     def leave_from_live_chat(self, chatId: str):
         if chatId in self.active_live_chats:
             self.active_live_chats.remove(chatId)
 
@@ -183,40 +184,40 @@
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
             },
             "t": 112
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "channelType": 1,
             },
             "t": 108
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
         self.active_live_chats.add(chatId)
         Thread(target=self.run_vc, args=(comId, chatId, joinType)).start()
 
     def end_vc(self, comId: int, chatId: str, joinType: int = 2):
         self.leave_from_live_chat(chatId)
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
             },
             "t": 112
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
         self.active_live_chats.remove(chatId)
 
     def Browsing(self, comId: int, blogId: str = None, blogType: int = 0):
         """
         Send Browsing Action
 
         **Paramaters**
@@ -237,15 +238,15 @@
                 "target": target,
                 "ndcId": int(comId),
                 "params": {"blogType": blogType},
             },
             "t": 306
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
     def Chatting(self, comId: int, chatId: str, threadType: int = 2):
         """
         Send Chatting Action
 
         **Paramaters**
             - **threadType**: 2 For Public 1 & 0 For Private (int)
@@ -263,15 +264,15 @@
                     "membershipStatus": 1,
                     "threadType": threadType
                 },
             },
             "t": 306
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
     def PublicChats(self, comId: int,):
         """
         Send PublicChats Action
 
         **Return**
             - **SetAction**:  (Class)
@@ -282,15 +283,15 @@
                 "target": f"ndc://x{comId}/public-chats",
                 "ndcId": int(comId),
                 "params": {"duration": 859},
             },
             "t": 306
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
     def LeaderBoards(self, comId: int,):
         """
         Send LeaderBoard Action
 
         **Return**
             - **SetAction**:  (Class)
@@ -301,39 +302,39 @@
                 "target": f"ndc://x{comId}/leaderboards",
                 "ndcId": int(comId),
                 "params": {"duration": 859},
             },
             "t": 306
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
     def start_video_chat(self, comId: str, chatId: str, joinType: int = 1):
         data = {
             "o": {
                 "ndcId": comId,
                 "threadId": chatId,
                 "joinRole": joinType,
             },
             "t": 112
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
                 "channelType": 4,
             },
             "t": 108
         }
         data = dumps(data)
-        self.socket.send(data)
+        self.send(data)
 
 
 class Callbacks:
     def __init__(self):
         self.handlers = {}
 
         self.methods = {
```

### Comparing `amino.light.py-0.1.1/AminoLightPy/sub_client.py` & `amino.light.py-0.1.2/AminoLightPy/sub_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,64 @@
+# pylint: disable=invalid-name
+
 from uuid import uuid4
 from time import timezone
+from typing import Union
+from typing import BinaryIO
 from requests import Session
-from base64 import b64encode
-from typing import BinaryIO, Union
 
 from .constants import api, upload_media
 from .lib.util import exceptions, objects
 
 
 class SubClient():
     def __init__(self, comId: int = None, *, profile: objects.UserProfile):
         self.vc_connect = False
         self.profile = profile
         self.session: Session = self.profile.session
 
         self.comId = comId
 
     def get_invite_codes(self, status: str = "normal", start: int = 0, size: int = 25):
-        response = self.session.get(f"{api}/g/s-x{self.comId}/community/invitation?status={status}&start={start}&size={size}")
+        """
+        Retrieves the invite codes for the community.
+
+        **Parameters**
+            - *status* : The status of the invite codes to be retrieved. Defaults to "normal".
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
+
+        **Returns**
+            - **Success** : :meth:`Invite Code List <AminoLightPy.lib.util.objects.InviteCodeList>`
+
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+        params = {
+            "status": status,
+            "start": start,
+            "size": size
+        }
+        response = self.session.get(f"{api}/g/s-x{self.comId}/community/invitation", params=params)
         return objects.InviteCodeList(response.json()["communityInvitationList"]).InviteCodeList
 
     def generate_invite_code(self, duration: int = 0, force: bool = True):
         data = {
             "duration": duration,
             "force": force
         }
-        
         response = self.session.post(f"{api}/g/s-x{self.comId}/community/invitation", json=data)
         return objects.InviteCode(response.json()["communityInvitation"]).InviteCode
 
     def delete_invite_code(self, inviteId: str):
         response = self.session.delete(f"{api}/g/s-x{self.comId}/community/invitation/{inviteId}")
         return response.status_code
 
-    def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False):
+    def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None,
+                        categoriesList: list = None, backgroundColor: str = None,
+                        fansOnly: bool = False, extensions: dict = None):
         mediaList = list()
 
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
                 mediaList.append([100, upload_media(self, image, "image"), caption])
 
         else:
@@ -55,35 +76,38 @@
             "longitude": 0,
             "eventSource": "GlobalComposeMenu",
         }
 
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
-        
         response = self.session.post(f"{api}/x{self.comId}/s/blog", json=data)
 
         return response.status_code
 
-    def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, props: list = [], backgroundMediaList: list = []):
-
+    def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None,
+                        keywords: str = None, backgroundColor: str = None, props: list = [],
+                        backgroundMediaList: list = []):
         data = {
             "label": title,
             "content": content,
             "mediaList": imageList,
             "eventSource": "GlobalComposeMenu",
             "extensions": {},
         }
-        
-        if icon: data["icon"] = icon
-        if keywords: data["keywords"] = keywords
-        if props: data["extensions"].update({"props": props})
-        if backgroundMediaList: data["extensions"].update({"style": {"backgroundMediaList": backgroundMediaList}})
-        if backgroundColor: data["extensions"].update({"style": {"backgroundColor": backgroundColor}})
-
+        if icon:
+            data["icon"] = icon
+        if keywords:
+            data["keywords"] = keywords
+        if props:
+            data["extensions"].update({"props": props})
+        if backgroundMediaList:
+            data["extensions"].update({"style": {"backgroundMediaList": backgroundMediaList}})
+        if backgroundColor:
+            data["extensions"].update({"style": {"backgroundColor": backgroundColor}})
 
         response = self.session.post(f"{api}/x{self.comId}/s/item", json=data)
         return response.status_code
 
     def edit_blog(self, blogId: str, title: str = None, content: str = None, imageList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False):
         mediaList = list()
 
@@ -99,15 +123,14 @@
         }
 
         if title: data["title"] = title
         if content: data["content"] = content
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
-        
         response = self.session.post(f"{api}/x{self.comId}/s/blog/{blogId}", json=data)
         return response.status_code
 
     def delete_blog(self, blogId: str):
         response = self.session.delete(f"{api}/x{self.comId}/s/blog/{blogId}")
         return response.status_code
 
@@ -122,81 +145,90 @@
 
         data = {
             "content": content,
             "refObjectId": refObjectId,
             "refObjectType": refObjectType,
             "type": 2,
         }
-        
         response = self.session.post(f"{api}/x{self.comId}/s/blog", json=data)
         return response.status_code
 
     def check_in(self, tz: int = -timezone // 1000):
         data = { "timezone": tz }
-        
         response = self.session.post(f"{api}/x{self.comId}/s/check-in", json=data)
         return response.status_code
 
     def repair_check_in(self, method: int = 0):
-        data = dict()
+        data = {}
         if method == 0: data["repairMethod"] = "1"  # Coins
         if method == 1: data["repairMethod"] = "2"  # Amino+
-        
         response = self.session.post(f"{api}/x{self.comId}/s/check-in/repair", json=data)
         return response.status_code
 
     def lottery(self, tz: int = -timezone // 1000):
         data = { "timezone": tz }
-        
         response = self.session.post(f"{api}/x{self.comId}/s/check-in/lottery", json=data)
         return objects.LotteryLog(response.json()["lotteryLog"]).LotteryLog
 
-    def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None):
-        mediaList = list()
-
-        data = dict()
-
+    def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None,
+                            chatRequestPrivilege: str = None, imageList: list = None,
+                            captionList: list = None, backgroundImage: str = None,
+                            backgroundColor: str = None, titles: list = None, colors: list = None,
+                            defaultBubbleId: str = None):
+        mediaList = []
+        data = {}
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
                 mediaList.append([100, upload_media(self, image, "image"), caption])
 
         else:
             if imageList is not None:
                 for image in imageList:
                     mediaList.append([100, upload_media(self, image, "image"), None])
 
         if imageList is not None or captionList is not None:
             data["mediaList"] = mediaList
 
-        if nickname: data["nickname"] = nickname
-        if icon: data["icon"] = upload_media(self, icon, "image")
-        if content: data["content"] = content
-
-        if chatRequestPrivilege: data["extensions"] = {"privilegeOfChatInviteRequest": chatRequestPrivilege}
-        if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
-        if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+        if nickname:
+            data["nickname"] = nickname
+        if icon:
+            data["icon"] = upload_media(self, icon, "image")
+        if content:
+            data["content"] = content
+
+        if chatRequestPrivilege:
+            data["extensions"] = {"privilegeOfChatInviteRequest": chatRequestPrivilege}
+        if backgroundImage:
+            data["extensions"] = {"style": {
+                "backgroundMediaList": [[100, backgroundImage, None, None, None]]
+                }}
+        if backgroundColor:
+            data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if defaultBubbleId:
+            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
 
         if titles or colors:
             tlt = []
             for titles, colors in zip(titles, colors):
                 tlt.append({"title": titles, "color": colors})
 
             data["extensions"] = {"customTitles": tlt}
-        
 
-        response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{self.profile.userId}", json=data)
+        response = self.session.post(
+            url=f"{api}/x{self.comId}/s/user-profile/{self.profile.userId}",
+            json=data
+        )
         return response.status_code
 
     def vote_poll(self, blogId: str, optionId: str):
         data = {
             "value": 1,
             "eventSource": "PostDetailView"
         }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", json=data)
         return response.status_code
 
     def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None, isGuest: bool = False):
         data = {
             "content": message,
             "stickerId": None,
@@ -242,15 +274,15 @@
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "value": 4
         }
 
         if blogId:
             if isinstance(blogId, str):
@@ -280,33 +312,35 @@
         response = self.session.delete(url)
         return response.status_code
 
     def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
         data = {
             "value": 1
         }
+        params = {
+            "cv": "1.2",
+            "value": "1"
+        }
 
         if userId:
             data["eventSource"] = "UserProfileView"
-            
-            url = f"{api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote?cv=1.2&value=1"
+            url = f"{api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote"
 
         elif blogId:
             data["eventSource"] = "PostDetailView"
-            
-            url = f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1"
+            url = f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote"
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
-            
-            url = f"{api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1"
+            url = f"{api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote"
 
-        else: raise exceptions.SpecifyType()
+        else:
+            raise exceptions.SpecifyType()
 
-        response = self.session.post(url, json=data)
+        response = self.session.post(url=url, json=data, params=params)
         return response.status_code
 
     def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
         if userId: url = f"{api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView"
         elif blogId: url = f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
         elif wikiId: url = f"{api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView"
         else: raise exceptions.SpecifyType()
@@ -315,60 +349,68 @@
         return response.status_code
 
     def upvote_comment(self, blogId: str, commentId: str):
         data = {
             "value": 1,
             "eventSource": "PostDetailView"
         }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", json=data)
         return response.status_code
 
     def downvote_comment(self, blogId: str, commentId: str):
         data = {
             "value": -1,
             "eventSource": "PostDetailView"
         }
-        
-        response = self.session.post(f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", json=data)
+        params = {
+            "cv": "1.2",
+            "value": "-1"
+        }
+
+        response = self.session.post(
+            url=f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote",
+            json=data,
+            params=params
+        )
         return response.status_code
 
     def unvote_comment(self, blogId: str, commentId: str):
         response = self.session.delete(f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?eventSource=PostDetailView")
         return response.status_code
 
     def reply_wall(self, userId: str, commentId: str, message: str):
         data = {
             "content": message,
             "stackedId": None,
             "respondTo": commentId,
             "type": 0,
             "eventSource": "UserProfileView"
         }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{userId}/comment", json=data)
         return response.status_code
 
-    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None): 
-        data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "optInAdsFlags": optInAdsFlags, "timezone": tz} 
-        if timers: data["userActiveTimeChunkList"] = timers 
-        
-        response = self.session.post(f"{api}/x{self.comId}/s/community/stats/user-active-time", json=data) 
+    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None):
+        data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "optInAdsFlags": optInAdsFlags, "timezone": tz}
+        if timers: data["userActiveTimeChunkList"] = timers
+
+        response = self.session.post(f"{api}/x{self.comId}/s/community/stats/user-active-time", json=data)
         return response.status_code
 
     def activity_status(self, status: str):
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
         else: raise exceptions.WrongType(status)
 
         data = {
             "onlineStatus": status,
             "duration": 86400
         }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", json=data)
         return response.status_code
 
     # TODO : Finish this
     def watch_ad(self):
         response = self.session.post(f"{api}/g/s/wallet/ads/video/start")
         return response.status_code
@@ -397,34 +439,33 @@
             "initialMessageContent": message,
             "content": content
         }
 
         if isGlobal is True:
             data["type"] = 2
             data["eventSource"] = "GlobalComposeMenu"
-        else: 
+        else:
             data["type"] = 0
 
-        if publishToGlobal is True: 
+        if publishToGlobal is True:
             data["publishToGlobal"] = 1
-        else: 
+        else:
             data["publishToGlobal"] = 0
 
-        
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread", json=data)
         return objects.Thread(response.json()["thread"]).Thread
 
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         elif isinstance(userId, tuple): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = { "uids": userIds }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/invite", json=data)
         return response.status_code
 
     def add_to_favorites(self, userId: str):
         response = self.session.post(f"{api}/x{self.comId}/s/user-group/quick-access/{userId}")
         return response.status_code
 
@@ -441,41 +482,46 @@
         if chatId is not None: url = f"{api}/x{self.comId}/s/chat/thread/{chatId}/tipping"
         if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
             url = f"{api}/x{self.comId}/s/tipping"
 
         if url is None: raise exceptions.SpecifyType
-        
+
         response = self.session.post(url, json=data)
         return response.status_code
 
     def thank_tip(self, chatId: str, userId: str):
-        response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank")
+        response = self.session.post(
+            url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank"
+        )
         return response.status_code
 
     def follow(self, userId: Union[str, list]):
         """
         Follow an User or Multiple Users.
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         if isinstance(userId, str):
             response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{userId}/member")
 
         elif isinstance(userId, list):
             data = { "targetUidList": userId }
-            
-            response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined", json=data)
+
+            response = self.session.post(
+                url=f"{api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined",
+                json=data
+            )
 
         else: raise exceptions.WrongType(type(userId))
 
         return response.status_code
 
     def unfollow(self, userId: str):
         """
@@ -483,45 +529,45 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.delete(f"{api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined/{userId}")
         return response.status_code
 
     def block(self, userId: str):
         """
         Block an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.post(f"{api}/x{self.comId}/s/block/{userId}")
         return response.status_code
 
     def unblock(self, userId: str):
         """
         Unblock an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.delete(f"{api}/x{self.comId}/s/block/{userId}")
         return response.status_code
 
     def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
         """
         Flag a User, Blog or Wiki.
@@ -533,15 +579,15 @@
             - **blogId** : ID of the Blog.
             - **wikiId** : ID of the Wiki.
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason
@@ -560,15 +606,14 @@
             data["objectType"] = 2
 
         else: raise exceptions.SpecifyType
 
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
-        
         response = self.session.post(f"{api}/x{self.comId}/s/{flg}", json=data)
         return response.status_code
 
     def check_values(self, *args):
         return any(arg is None for arg in args)
 
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
@@ -590,25 +635,24 @@
             - **embedLink** : Link of the Embed.
             - **embedImage** : Image of the Embed.
             - **embedId** : ID of the Embed.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        
 
         data = {
             "type": messageType,
             "content": message
         }
-        
+
         if self.check_values(embedId, embedType, embedLink, embedTitle, embedContent, embedImage):
-            attachedObject = dict()
+            attachedObject = {}
 
             if embedId:
                 attachedObject["objectId"] = embedId
 
             if embedType:
                 attachedObject["objectType"] = embedType
 
@@ -621,15 +665,15 @@
             if embedContent:
                 attachedObject["content"] = embedContent
 
             if embedImage:
                 attachedObject["mediaList"] = [[100, upload_media(self, embedImage, "image"), None]]
 
             data["attachedObject"] = attachedObject
-        
+
         if mentionUserIds:
             mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
             data["extensions"] = {"mentionedArray": mentions}
 
         if replyTo: data["replyMessageId"] = replyTo
 
         if stickerId:
@@ -639,32 +683,30 @@
 
         if file:
             data["content"] = None
             url = upload_media(self, file, fileType)
 
             data["mediaValue"] = url
 
-
         response = self.session.post(
             url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/message",
             json=data
         )
 
         return response.status_code
 
     def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
+        url = upload_media(self, image, "image/png")
         data = {
             "type": 0,
             "content": message,
             "extensions": {
                 "linkSnippetList": [{
                     "link": link,
-                    "mediaType": 100,
-                    "mediaUploadValue": b64encode(image.read()).decode(),
-                    "mediaUploadValueContentType": "image/png"
+                    "mediaValue": url
                 }]
             },
             "attachedObject": None
         }
         
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/message", json=data)
         return response.status_code
@@ -678,46 +720,47 @@
             - **chatId** : ID of the Chat.
             - **asStaff** : If execute as a Staff member (Leader or Curator).
             - **reason** : Reason of the action to show on the Moderation History.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "adminOpName": 102,
         }
 
         if asStaff and reason:
             data["adminOpNote"] = {"content": reason}
 
-        
-        if not asStaff: response = self.session.delete(f"{api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}")
-        else: response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}/admin", json=data)
+        if not asStaff:
+            response = self.session.delete(f"{api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}")
+        else:
+            response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}/admin", json=data)
 
         return response.status_code
 
     def mark_as_read(self, chatId: str, messageId: str):
         """
         Mark a Message from a Chat as Read.
 
         **Parameters**
             - **messageId** : ID of the Message.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         data = {
             "messageId": messageId
         }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", json=data)
         return response.status_code
 
     def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None, title: str = None, icon: str = None, backgroundImage: str = None, content: str = None, announcement: str = None, coHosts: list = None, keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None, canTip: bool = None, viewOnly: bool = None, canInvite: bool = None, fansOnly: bool = None):
         """
         Send a Message to a Chat.
 
@@ -738,17 +781,17 @@
             - **publishToGlobal** : If the Chat should show on Public Chats or not.
             - **doNotDisturb** : If the Chat should Do Not Disturb or not.
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
-        data = dict()
+        data = {}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if announcement: data["extensions"] = {"announcement": announcement}
         if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
@@ -758,42 +801,42 @@
         if not publishToGlobal: data["publishToGlobal"] = 1
 
         res = list()
 
         if doNotDisturb is not None:
             if doNotDisturb:
                 data = {"alertOption": 2 }
-                
+
                 response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", json=data)
                 res.append(response.status_code)
 
             if not doNotDisturb:
                 data = {"alertOption": 1 }
-                
+
                 response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", json=data)
                 res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
                 response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/pin", json=data)
                 res.append(response.status_code)
 
             if not pinChat:
                 response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/unpin", json=data)
                 res.append(response.status_code)
 
         if backgroundImage is not None:
             data = {"media": [100, backgroundImage, None] }
-            
+
             response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/background", json=data)
             res.append(response.status_code)
 
         if coHosts is not None:
             data = {"uidList": coHosts }
-            
+
             response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/co-host", json=data)
             res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
                 response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/view-only/enable")
                 res.append(response.status_code)
@@ -816,112 +859,147 @@
                 response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/enable", json=data)
                 res.append(response.status_code)
 
             if not canTip:
                 response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/disable", json=data)
                 res.append(response.status_code)
 
-        
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}", json=data)
         res.append(response.status_code)
 
         return res
 
     def transfer_host(self, chatId: str, userIds: list):
         data = { "uidList": userIds }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", json=data)
         return response.status_code
 
     def transfer_organizer(self, chatId: str, userIds: list):
         self.transfer_host(chatId, userIds)
 
     def accept_host(self, chatId: str, requestId: str):
-        data = dict()
-        
-        response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", json=data)
+        """
+        Accepts a host request for a chat.
+
+        **Parameters**
+            - **chatId** (str): ID of the chat.
+            - **requestId** (str): ID of the host request.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+        response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept")
         return response.status_code
 
     def accept_organizer(self, chatId: str, requestId: str):
+        """
+        Accepts a host request for a chat.
+
+        **Parameters**
+            - **chatId** (str): ID of the chat.
+            - **requestId** (str): ID of the host request.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         self.accept_host(chatId, requestId)
 
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
-        if allowRejoin: allowRejoin = 1
-        if not allowRejoin: allowRejoin = 0
-        response = self.session.delete(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}")
+        """
+        Kicks a user from a chat.
+
+        **Parameters**
+            - **userId** (str): ID of the user to be kicked.
+            - **chatId** (str): ID of the chat from which the user is to be kicked.
+            - *allowRejoin* (bool, optional): Whether the user is allowed to rejoin the chat. Defaults to True.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+
+        params = {"allowRejoin": int(allowRejoin)}
+
+        response = self.session.delete(
+            url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/{userId}",
+            params=params
+        )
         return response.status_code
 
     def join_chat(self, chatId: str):
         """
         Join an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}")
         return response.status_code
 
     def leave_chat(self, chatId: str):
         """
         Leave an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.delete(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}")
         return response.status_code
-        
+
     def delete_chat(self, chatId: str):
         """
         Delete a Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.delete(f"{api}/x{self.comId}/s/chat/thread/{chatId}")
         return response.status_code
-        
+
     def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None):
         if transactionId is None: transactionId = str(uuid4())
 
         data = {
             "paymentContext": {
                 "transactionId": transactionId,
                 "isAutoRenew": autoRenew
             }
         }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/influencer/{userId}/subscribe", json=data)
         return response.status_code
 
     def promotion(self, noticeId: str, type: str = "accept"):
         response = self.session.post(f"{api}/x{self.comId}/s/notice/{noticeId}/{type}")
         return response.status_code
 
     def play_quiz_raw(self, quizId: str, quizAnswerList: list, quizMode: int = 0):
         data = {
             "mode": quizMode,
             "quizAnswerList": quizAnswerList
         }
-        
+
         response = self.session.post(f"{api}/x{self.comId}/s/blog/{quizId}/quiz/result", json=data)
         return response.status_code
 
     def play_quiz(self, quizId: str, questionIdsList: list, answerIdsList: list, quizMode: int = 0):
         quizAnswerList = list()
 
         for question, answer in zip(questionIdsList, answerIdsList):
@@ -933,27 +1011,28 @@
 
             quizAnswerList.append(part)
 
         data = {
             "mode": quizMode,
             "quizAnswerList": quizAnswerList
         }
-        
         response = self.session.post(f"{api}/x{self.comId}/s/blog/{quizId}/quiz/result", json=data)
         return response.status_code
 
     def vc_permission(self, chatId: str, permission: int):
         """Voice Chat Join Permissions
         1 - Open to Everyone
         2 - Approval Required
         3 - Invite Only
         """
         data = { "vvChatJoinType": permission }
-        
-        response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", json=data)
+        response = self.session.post(
+            url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission",
+            json=data
+        )
         return response.status_code
 
     def get_vc_reputation_info(self, chatId: str):
         response = self.session.get(f"{api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation")
         return objects.VcReputation(response.json()).VcReputation
 
     def claim_vc_reputation(self, chatId: str):
@@ -981,87 +1060,87 @@
         """
         Information of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+            - **Success** : :meth:`User Object <AminoLightPy.lib.util.objects.UserProfile>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/user-profile/{userId}")
         return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
     def get_user_following(self, userId: str, start: int = 0, size: int = 25):
         """
         List of Users that the User is Following.
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <AminoLightPy.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}")
         return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
         """
         List of Users that are Following the User.
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <AminoLightPy.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}")
         return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_user_checkins(self, userId: str):
         response = self.session.get(f"{api}/x{self.comId}/s/check-in/stats/{userId}?timezone={timezone // 1000}")
         return objects.UserCheckIns(response.json()).UserCheckIns
 
     def get_user_blogs(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{api}/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{api}/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}")
         return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_user_wikis(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{api}/x{self.comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}", headers=self.parse_headers())
+        response = self.session.get(f"{api}/x{self.comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}")
         return objects.WikiList(response.json()["itemList"]).WikiList
 
     def get_user_achievements(self, userId: str):
-        response = self.session.get(f"{api}/x{self.comId}/s/user-profile/{userId}/achievements", headers=self.parse_headers())
+        response = self.session.get(f"{api}/x{self.comId}/s/user-profile/{userId}/achievements")
         return objects.UserAchievements(response.json()["achievements"]).UserAchievements
 
     def get_influencer_fans(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{api}/x{self.comId}/s/influencer/{userId}/fans?start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{api}/x{self.comId}/s/influencer/{userId}/fans?start={start}&size={size}")
         return objects.InfluencerFans(response.json()).InfluencerFans
 
     def get_blocked_users(self, start: int = 0, size: int = 25):
         """
         List of Users that the User Blocked.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`Users List <AminoLightPy.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/block?start={start}&size={size}")
         return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_blocker_users(self, start: int = 0, size: int = 25):
         """
         List of Users that are Blocking the User.
@@ -1069,15 +1148,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List of User IDs <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         response = self.session.get(f"{api}/x{self.comId}/s/block?start={start}&size={size}")
         return response.json()["blockerUidList"]
 
     def search_users(self, nickname: str, start: int = 0, size: int = 25):
         response = self.session.get(f"{api}/x{self.comId}/s/user-profile?type=name&q={nickname}&start={start}&size={size}")
@@ -1149,65 +1228,65 @@
         List of Chats the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <AminoLightPy.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}")
         return objects.ThreadList(response.json()["threadList"]).ThreadList
 
     def get_public_chat_threads(self, type: str = "recommended", start: int = 0, size: int = 25):
         """
         List of Public Chats of the Community.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <AminoLightPy.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}")
         return objects.ThreadList(response.json()["threadList"]).ThreadList
 
     def get_chat_thread(self, chatId: str):
         """
         Get the Chat Object from an Chat ID.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+            - **Success** : :meth:`Chat Object <AminoLightPy.lib.util.objects.Thread>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/chat/thread/{chatId}")
         return objects.Thread(response.json()["thread"]).Thread
 
     def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
         """
         List of Messages from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+            - **Success** : :meth:`Message List <AminoLightPy.lib.util.objects.MessageList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         if pageToken is not None: url = f"{api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"{api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
         response = self.session.get(url)
         return objects.GetMessages(response.json()).GetMessages
@@ -1217,17 +1296,17 @@
         Information of an Message from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - **message** : ID of the Message.
 
         **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+            - **Success** : :meth:`Message Object <AminoLightPy.lib.util.objects.Message>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         response = self.session.get(f"{api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}")
         return objects.Message(response.json()["message"]).Message
 
     def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
         if blogId or quizId:
             if quizId is not None: blogId = quizId
@@ -1286,17 +1365,17 @@
             - **userId** : ID of the User.
             - **sorting** : Order of the Comments.
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : :meth:`Comments List <AminoLightPy.lib.util.objects.CommentList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
         response = self.session.get(f"{api}/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}")
@@ -1306,15 +1385,33 @@
         if pageToken is not None: url = f"{api}/x{self.comId}/s/feed/blog-all?pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"{api}/x{self.comId}/s/feed/blog-all?pagingType=t&start={start}&size={size}"
 
         response = self.session.get(url)
         return objects.RecentBlogs(response.json()).RecentBlogs
 
     def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2")
+        """
+        List of users in a chat.
+
+        **Parameters**
+            - **chatId** (str): ID of the chat.
+            - *start* (int, optional): The index from which to start the list. Defaults to 0.
+            - *size* (int, optional): The size of the list. Defaults to 25.
+
+        **Returns**
+            - **Success** : :meth:`User List <AminoLightPy.lib.util.objects.UserProfileList>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
+        params = {
+            "start": start,
+            "size": size,
+            "type": "default",
+            "cv": "1.2"
+        }
+        response = self.session.get(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member", params=params)
         return objects.UserProfileList(response.json()["memberList"]).UserProfileList
 
     def get_notifications(self, start: int = 0, size: int = 25):
         response = self.session.get(f"{api}/x{self.comId}/s/notification?pagingType=t&start={start}&size={size}")
         return objects.NotificationList(response.json()["notificationList"]).NotificationList
 
     def get_notices(self, start: int = 0, size: int = 25):
@@ -1577,20 +1674,26 @@
         }
 
         response = self.session.post(f"{api}/x{self.comId}/s/notice", json=data)
         return response.json()
 
     # TODO : List all strike texts
     def strike(self, userId: str, time: int, title: str = None, reason: str = None):
-        if time == 1: time = 86400
-        elif time == 2: time = 10800
-        elif time == 3: time = 21600
-        elif time == 4: time = 43200
-        elif time == 5: time = 86400
-        else: raise exceptions.WrongType(time)
+        if time == 1:
+            time = 86400
+        elif time == 2:
+            time = 10800
+        elif time == 3:
+            time = 21600
+        elif time == 4:
+            time = 43200
+        elif time == 5:
+            time = 86400
+        else:
+            raise exceptions.WrongType(time)
 
         data = {
             "uid": userId,
             "title": title,
             "content": reason,
             "attachedObject": {
                 "objectId": userId,
@@ -1654,22 +1757,35 @@
 
     def get_best_quiz(self, start: int = 0, size: int = 25):
         response = self.session.get(f"{api}/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}")
         return objects.BlogList(response.json()["blogList"]).BlogList
 
     # Provided by "spectrum#4691"
     def purchase(self, objectId: str, objectType: int, aminoPlus: bool = True, autoRenew: bool = False):
+        """
+        Makes a purchase in the store.
+
+        **Parameters**
+            - **objectId** (str): ID of the object to be purchased.
+            - *isAutoRenew* (bool, optional): Whether the purchase should be auto-renewed. Defaults to False.
+
+        **Returns**
+            - **Success** : 200 (int)
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
+        """
         data = {
             "objectId": objectId,
             "objectType": objectType,
             "v": 1,
         }
 
-        if aminoPlus: data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
-        else: data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
+        if aminoPlus:
+            data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
+        else:
+            data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
 
         response = self.session.post(f"{api}/x{self.comId}/s/store/purchase", json=data)
         return response.status_code
 
     # Provided by "spectrum#4691"
     def apply_avatar_frame(self, avatarId: str, applyToAll: bool = True):
         """
@@ -1678,15 +1794,15 @@
         **Parameters**
             - **avatarId** : ID of the avatar frame.
             - **applyToAll** : Apply to all.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
 
         """
 
         data = {
             "frameId": avatarId,
             "applyToAll": 0,
         }
@@ -1703,15 +1819,15 @@
         **Parameters**
             - **chatId** - ID of the Chat
             - **userId** - ID of the User
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>`
         """
 
         data = { "uid": userId }
 
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", json=data)
         return response.status_code
 
@@ -1757,15 +1873,15 @@
             "actionType": "create"
         }
 
         response = self.session.post(f"{api}/x{self.comId}/s/knowledge-base-request/{requestId}/approve", json=data)
         return response.status_code
 
     def reject_wiki_request(self, requestId: str):
-        data = dict()
+        data = {}
 
         response = self.session.post(f"{api}/x{self.comId}/s/knowledge-base-request/{requestId}/reject", json=data)
         return response.status_code
 
     def get_wiki_submissions(self, start: int = 0, size: int = 25):
         response = self.session.get(f"{api}/x{self.comId}/s/knowledge-base-request?type=all&start={start}&size={size}")
         return objects.WikiRequestList(response.json()["knowledgeBaseRequestList"]).WikiRequestList
```

### Comparing `amino.light.py-0.1.1/LICENSE` & `amino.light.py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.1/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.2/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.1/setup.py` & `amino.light.py-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 keywords = [
     'amino',
     'aminoapps',
     'amino.fix',
     'amino.light',
     'amino.ligt.py',
     'AminoLightPy',
-    'amino',
     'amino-bot',
     'narvii',
     'medialab',
     'api',
     'python',
     'python3',
     'python3.x',
     'minori',
     'august',
     'augustlight',
-    'aminolightpy'
+    'aminolightpy',
+    'amino.py'
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.1",
+    version="0.1.2",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
```

