# Comparing `tmp/bring-api-0.6.0.tar.gz` & `tmp/bring-api-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring-api-0.6.0.tar", last modified: Fri Apr  5 16:06:28 2024, max compression
+gzip compressed data, was "bring-api-0.7.0.tar", last modified: Wed Apr 10 11:38:34 2024, max compression
```

## Comparing `bring-api-0.6.0.tar` & `bring-api-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.403682 bring-api-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-05 16:06:20.000000 bring-api-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 16:06:20.000000 bring-api-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-05 16:06:28.403682 bring-api-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-05 16:06:20.000000 bring-api-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.395682 bring-api-0.6.0/bring_api/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41753 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/bring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.399682 bring-api-0.6.0/bring_api/locales/
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.de-AT.json
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.de-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.de-DE.json
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-AU.json
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-CA.json
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-GB.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-US.json
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.es-ES.json
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.fr-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.fr-FR.json
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.hu-HU.json
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.it-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.it-IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.nb-NO.json
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.nl-NL.json
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.pl-PL.json
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.pt-BR.json
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.ru-RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.sv-SE.json
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.tr-TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.399682 bring-api-0.6.0/bring_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-05 16:06:20.000000 bring-api-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-05 16:06:28.403682 bring-api-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.399682 bring-api-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    38934 2024-04-05 16:06:20.000000 bring-api-0.6.0/tests/test_bring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-10 11:38:29.000000 bring-api-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-10 11:38:29.000000 bring-api-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-10 11:38:34.161381 bring-api-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-10 11:38:29.000000 bring-api-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.153381 bring-api-0.7.0/bring_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53071 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/bring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/bring_api/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.de-AT.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.de-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.de-DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-AU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-CA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-US.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.es-ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.fr-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.fr-FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.hu-HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.it-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.it-IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.nb-NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.nl-NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.pl-PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.pt-BR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.ru-RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.sv-SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.tr-TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/bring_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-10 11:38:29.000000 bring-api-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 11:38:34.161381 bring-api-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    45727 2024-04-10 11:38:29.000000 bring-api-0.7.0/tests/test_bring.py
```

### Comparing `bring-api-0.6.0/CHANGELOG.md` & `bring-api-0.7.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+# 0.7.0
+
+* **New API method:** `retrieve_new_access_token` retrieves a new access token and updates authorization headers. Time till expiration of the access token is stored in the property `expires_in` . ([tr4nt0r](https://github.com/tr4nt0r))
+* All API methods that require authentication now raise `BringAuthException` for 401 Unauthorized status ([tr4nt0r](https://github.com/tr4nt0r))
+
 ## 0.6.0
 
 * **Pytest unit testing:** added pytest with full code coverage ([tr4nt0r](https://github.com/tr4nt0r))
 * **Github workflow for pytest:** added workflow for running pytests with Python 3.11 & 3.12 on Ubuntu, Windows and macOS ([tr4nt0r](https://github.com/tr4nt0r))
 * Update Python requirement to >=3.11
 * Change from implicit to explicit string conversion of `BringItemOperation` in JSON request payload ([tr4nt0r](https://github.com/tr4nt0r))
 * Change Type of `BringItemOperation` to `StrEnum` ([tr4nt0r](https://github.com/tr4nt0r))
```

### Comparing `bring-api-0.6.0/LICENSE` & `bring-api-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/PKG-INFO` & `bring-api-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -261,14 +261,19 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+# 0.7.0
+
+* **New API method:** `retrieve_new_access_token` retrieves a new access token and updates authorization headers. Time till expiration of the access token is stored in the property `expires_in` . ([tr4nt0r](https://github.com/tr4nt0r))
+* All API methods that require authentication now raise `BringAuthException` for 401 Unauthorized status ([tr4nt0r](https://github.com/tr4nt0r))
+
 ## 0.6.0
 
 * **Pytest unit testing:** added pytest with full code coverage ([tr4nt0r](https://github.com/tr4nt0r))
 * **Github workflow for pytest:** added workflow for running pytests with Python 3.11 & 3.12 on Ubuntu, Windows and macOS ([tr4nt0r](https://github.com/tr4nt0r))
 * Update Python requirement to >=3.11
 * Change from implicit to explicit string conversion of `BringItemOperation` in JSON request payload ([tr4nt0r](https://github.com/tr4nt0r))
 * Change Type of `BringItemOperation` to `StrEnum` ([tr4nt0r](https://github.com/tr4nt0r))
```

### Comparing `bring-api-0.6.0/README.md` & `bring-api-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/bring.py` & `bring-api-0.7.0/bring_api/bring.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Bring api implementation."""
 
 import asyncio
+from http import HTTPStatus
 import json
 from json import JSONDecodeError
 import logging
 import os
+import time
 import traceback
 from typing import Any, List, Optional, cast
 
 import aiohttp
 
 from .const import (
     API_BASE_URL,
@@ -24,14 +26,15 @@
     BringParseException,
     BringRequestException,
     BringTranslationException,
     BringUserUnknownException,
 )
 from .types import (
     BringAuthResponse,
+    BringAuthTokenRespone,
     BringItem,
     BringItemOperation,
     BringItemsResponse,
     BringListItemDetails,
     BringListItemsDetailsResponse,
     BringListResponse,
     BringNotificationsConfigType,
@@ -62,17 +65,28 @@
         self.user_locale = BRING_DEFAULT_LOCALE
 
         self.__translations: dict[str, dict[str, str]] = {}
         self.uuid = ""
 
         self.url = API_BASE_URL
 
-        self.headers = DEFAULT_HEADERS
+        self.headers = DEFAULT_HEADERS.copy()
 
         self.loop = asyncio.get_running_loop()
+        self.refresh_token = ""
+        self.__expires_in: int
+
+    @property
+    def expires_in(self) -> int:
+        """Refresh token expiration."""
+        return max(0, self.__expires_in - int(time.time()))
+
+    @expires_in.setter
+    def expires_in(self, expires_in: int | str) -> None:
+        self.__expires_in = int(time.time()) + int(expires_in)
 
     async def login(self) -> BringAuthResponse:
         """Try to login.
 
         Returns
         -------
         Response
@@ -92,31 +106,32 @@
         user_data = {"email": self.mail, "password": self.password}
 
         try:
             url = f"{self.url}v2/bringauth"
             async with self._session.post(url, data=user_data) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
 
-                if r.status == 401:
+                if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.error(
                             "Exception: Cannot parse login request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
-                            "Login failed due to authorization failure but error response could not be parsed."
+                            "Login failed due to authorization failure "
+                            "but error response could not be parsed."
                         ) from e
                     _LOGGER.error("Exception: Cannot login: %s", errmsg["message"])
                     raise BringAuthException(
                         "Login failed due to authorization failure, "
                         "please check your email and password."
                     )
-                if r.status == 400:
+                if r.status == HTTPStatus.BAD_REQUEST:
                     _LOGGER.error("Exception: Cannot login: %s", await r.text())
                     raise BringAuthException(
                         "Login failed due to bad request, please check your email."
                     )
                 r.raise_for_status()
 
                 try:
@@ -145,15 +160,17 @@
             raise BringRequestException(
                 "Authentication failed due to request exception."
             ) from e
 
         self.uuid = data["uuid"]
         self.public_uuid = data.get("publicUuid", "")
         self.headers["X-BRING-USER-UUID"] = self.uuid
-        self.headers["Authorization"] = f'Bearer {data["access_token"]}'
+        self.headers["Authorization"] = f'{data["token_type"]} {data["access_token"]}'
+        self.refresh_token = data["refresh_token"]
+        self.expires_in = data["expires_in"]
 
         locale = (await self.get_user_account())["userLocale"]
         self.headers["X-BRING-COUNTRY"] = locale["country"]
         self.user_locale = self.map_user_language_to_locale(locale)
 
         self.user_list_settings = await self.__load_user_list_settings()
 
@@ -178,14 +195,36 @@
             If the parsing of the request response fails.
 
         """
         try:
             url = f"{self.url}bringusers/{self.uuid}/lists"
             async with self._session.get(url, headers=self.headers) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
+
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Loading lists failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot get lists: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Loading lists failed due to authorization failure, "
+                        "the authorization token is invalid or expired."
+                    )
+
                 r.raise_for_status()
 
                 try:
                     data = cast(
                         BringListResponse,
                         {
                             key: val
@@ -233,14 +272,36 @@
             If the parsing of the request response fails.
 
         """
         try:
             url = f"{self.url}v2/bringlists/{list_uuid}"
             async with self._session.get(url, headers=self.headers) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
+
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Loading list items failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot get list items: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Loading list items failed due to authorization failure, "
+                        "the authorization token is invalid or expired."
+                    )
+
                 r.raise_for_status()
 
                 try:
                     data = cast(
                         BringItemsResponse,
                         {
                             key: val
@@ -312,14 +373,36 @@
             If the parsing of the request response fails.
 
         """
         try:
             url = f"{self.url}bringlists/{list_uuid}/details"
             async with self._session.get(url, headers=self.headers) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
+
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Loading list details failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot get list details: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Loading list details failed due to authorization failure, "
+                        "the authorization token is invalid or expired."
+                    )
+
                 r.raise_for_status()
 
                 try:
                     data = [
                         cast(
                             BringListItemDetails,
                             {
@@ -619,14 +702,36 @@
             json_data["arguments"] = [item_name]
         try:
             url = f"{self.url}v2/bringnotifications/lists/{list_uuid}"
             async with self._session.post(
                 url, headers=self.headers, json=json_data
             ) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
+
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Sending notification failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot send notification: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Sending notification failed due to authorization failure, "
+                        "the authorization token is invalid or expired."
+                    )
+
                 r.raise_for_status()
                 return r
         except asyncio.TimeoutError as e:
             _LOGGER.error(
                 "Exception: Cannot send notification %s for list %s:\n%s",
                 notification_type,
                 list_uuid,
@@ -679,15 +784,15 @@
         params = {"email": mail}
 
         try:
             url = f"{self.url}bringusers"
             async with self._session.get(url, headers=self.headers, params=params) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
 
-                if r.status == 404:
+                if r.status == HTTPStatus.NOT_FOUND:
                     _LOGGER.error("Exception: User %s does not exist.", mail)
                     raise BringUserUnknownException(f"User {mail} does not exist.")
 
                 r.raise_for_status()
 
         except asyncio.TimeoutError as e:
             _LOGGER.error(
@@ -914,14 +1019,36 @@
             If the parsing of the request response fails.
 
         """
         try:
             url = f"{self.url}bringusersettings/{self.uuid}"
             async with self._session.get(url, headers=self.headers) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
+
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Loading user settings failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot get user settings: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Loading user settings failed due to authorization failure, "
+                        "the authorization token is invalid or expired."
+                    )
+
                 r.raise_for_status()
 
                 try:
                     usersettings = [
                         cast(
                             BringUserSettingsEntry,
                             {
@@ -1065,14 +1192,36 @@
             If the parsing of the request response fails.
 
         """
         try:
             url = f"{self.url}v2/bringusers/{self.uuid}"
             async with self._session.get(url, headers=self.headers) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
+
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Loading current user settings failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot get current user settings: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Loading current user settings failed due to authorization failure, "
+                        "the authorization token is invalid or expired."
+                    )
+
                 r.raise_for_status()
 
                 try:
                     data = cast(
                         BringSyncCurrentUserResponse,
                         {
                             key: val
@@ -1164,14 +1313,36 @@
 
         try:
             url = f"{self.url}v2/bringlists/{list_uuid}/items"
             async with self._session.put(
                 url, headers=self.headers, json=json_data
             ) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
+
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Batch operation failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot get execute batch operation: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Batch operation failed due to authorization failure, "
+                        "the authorization token is invalid or expired."
+                    )
+
                 r.raise_for_status()
                 return r
         except asyncio.TimeoutError as e:
             _LOGGER.error(
                 "Exception: Cannot execute batch operations for list %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
@@ -1184,7 +1355,93 @@
                 "Exception: Cannot execute batch operations for %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 f"Batch operation for list {list_uuid} failed due to request exception."
             ) from e
+
+    async def retrieve_new_access_token(
+        self, refresh_token: str | None = None
+    ) -> BringAuthTokenRespone:
+        """Refresh the access token.
+
+        Parameters
+        ----------
+        refresh_token : str, optional
+            The refresh token to use to retrieve a new access token
+
+        Returns
+        -------
+        dict
+            The JSON response as a dict.
+
+        Raises
+        ------
+        BringRequestException
+            If the request fails.
+
+        """
+        refresh_token = refresh_token or self.refresh_token
+
+        user_data = {"grant_type": "refresh_token", "refresh_token": refresh_token}
+        try:
+            url = f"{self.url}v2/bringauth/token"
+            async with self._session.post(
+                url, headers=self.headers, data=user_data
+            ) as r:
+                _LOGGER.debug("Response from %s: %s", url, r.status)
+                if r.status == HTTPStatus.UNAUTHORIZED:
+                    try:
+                        errmsg = await r.json()
+                    except JSONDecodeError as e:
+                        _LOGGER.error(
+                            "Exception: Cannot parse token request response:\n %s",
+                            traceback.format_exc(),
+                        )
+                        raise BringParseException(
+                            "Retrieve new access token failed due to authorization failure but "
+                            "error response could not be parsed."
+                        ) from e
+                    _LOGGER.error(
+                        "Exception: Cannot retrieve new access token: %s",
+                        errmsg["message"],
+                    )
+                    raise BringAuthException(
+                        "Retrieve new access token failed due to authorization failure, "
+                        "the refresh token is invalid or expired."
+                    )
+
+                r.raise_for_status()
+
+                try:
+                    data = cast(
+                        BringAuthTokenRespone,
+                        {
+                            key: val
+                            for key, val in (await r.json()).items()
+                            if key in BringAuthTokenRespone.__annotations__
+                        },
+                    )
+                except JSONDecodeError as e:
+                    _LOGGER.error(
+                        "Exception: Cannot retrieve new access token:\n %s",
+                        traceback.format_exc(),
+                    )
+                    raise BringParseException(
+                        "Cannot parse token request response."
+                    ) from e
+        except asyncio.TimeoutError as e:
+            _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
+            raise BringRequestException(
+                "Retrieve new access token failed due to connection timeout."
+            ) from e
+        except aiohttp.ClientError as e:
+            _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
+            raise BringRequestException(
+                "Retrieve new access token failed due to request exception."
+            ) from e
+
+        self.headers["Authorization"] = f'{data["token_type"]} {data["access_token"]}'
+        self.expires_in = data["expires_in"]
+
+        return data
```

### Comparing `bring-api-0.6.0/bring_api/const.py` & `bring-api-0.7.0/bring_api/const.py`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/exceptions.py` & `bring-api-0.7.0/bring_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.de-AT.json` & `bring-api-0.7.0/bring_api/locales/articles.de-AT.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.de-CH.json` & `bring-api-0.7.0/bring_api/locales/articles.de-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.de-DE.json` & `bring-api-0.7.0/bring_api/locales/articles.de-DE.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.en-AU.json` & `bring-api-0.7.0/bring_api/locales/articles.en-AU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.en-CA.json` & `bring-api-0.7.0/bring_api/locales/articles.en-CA.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.en-GB.json` & `bring-api-0.7.0/bring_api/locales/articles.en-GB.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.en-US.json` & `bring-api-0.7.0/bring_api/locales/articles.en-US.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.es-ES.json` & `bring-api-0.7.0/bring_api/locales/articles.es-ES.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.fr-CH.json` & `bring-api-0.7.0/bring_api/locales/articles.fr-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.fr-FR.json` & `bring-api-0.7.0/bring_api/locales/articles.fr-FR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.hu-HU.json` & `bring-api-0.7.0/bring_api/locales/articles.hu-HU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.it-CH.json` & `bring-api-0.7.0/bring_api/locales/articles.it-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.it-IT.json` & `bring-api-0.7.0/bring_api/locales/articles.it-IT.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.nb-NO.json` & `bring-api-0.7.0/bring_api/locales/articles.nb-NO.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.nl-NL.json` & `bring-api-0.7.0/bring_api/locales/articles.nl-NL.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.pl-PL.json` & `bring-api-0.7.0/bring_api/locales/articles.pl-PL.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.pt-BR.json` & `bring-api-0.7.0/bring_api/locales/articles.pt-BR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.ru-RU.json` & `bring-api-0.7.0/bring_api/locales/articles.ru-RU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.sv-SE.json` & `bring-api-0.7.0/bring_api/locales/articles.sv-SE.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/locales/articles.tr-TR.json` & `bring-api-0.7.0/bring_api/locales/articles.tr-TR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/bring_api/types.py` & `bring-api-0.7.0/bring_api/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,7 +140,16 @@
 
     itemId: str
     spec: str
     uuid: str
     operation: NotRequired[
         BringItemOperation | Literal["TO_PURCHASE", "TO_RECENTLY", "REMOVE"]
     ]
+
+
+class BringAuthTokenRespone(TypedDict):
+    """A refresh token response class."""
+
+    access_token: str
+    refresh_token: str
+    token_type: str
+    expires_in: int
```

### Comparing `bring-api-0.6.0/bring_api.egg-info/PKG-INFO` & `bring-api-0.7.0/bring_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -261,14 +261,19 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+# 0.7.0
+
+* **New API method:** `retrieve_new_access_token` retrieves a new access token and updates authorization headers. Time till expiration of the access token is stored in the property `expires_in` . ([tr4nt0r](https://github.com/tr4nt0r))
+* All API methods that require authentication now raise `BringAuthException` for 401 Unauthorized status ([tr4nt0r](https://github.com/tr4nt0r))
+
 ## 0.6.0
 
 * **Pytest unit testing:** added pytest with full code coverage ([tr4nt0r](https://github.com/tr4nt0r))
 * **Github workflow for pytest:** added workflow for running pytests with Python 3.11 & 3.12 on Ubuntu, Windows and macOS ([tr4nt0r](https://github.com/tr4nt0r))
 * Update Python requirement to >=3.11
 * Change from implicit to explicit string conversion of `BringItemOperation` in JSON request payload ([tr4nt0r](https://github.com/tr4nt0r))
 * Change Type of `BringItemOperation` to `StrEnum` ([tr4nt0r](https://github.com/tr4nt0r))
```

### Comparing `bring-api-0.6.0/bring_api.egg-info/SOURCES.txt` & `bring-api-0.7.0/bring_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/pyproject.toml` & `bring-api-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bring-api-0.6.0/setup.cfg` & `bring-api-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bring-api
-version = 0.6.0
+version = 0.7.0
 author = Cyrill Raccaud
 author_email = cyrill.raccaud+pypi@gmail.com
 description = Unofficial package to access Bring! shopping lists API.
 long_description = file: README.md, CHANGELOG.md, LICENCE
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/miaucl/python-bring-api
```

### Comparing `bring-api-0.6.0/tests/test_bring.py` & `bring-api-0.7.0/tests/test_bring.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Unit tests for bring-api."""
 
 import asyncio
 import enum
+from http import HTTPStatus
+import time
 
 import aiohttp
 from dotenv import load_dotenv
 import pytest
 
 from bring_api.bring import Bring
 from bring_api.const import BRING_SUPPORTED_LOCALES, DEFAULT_HEADERS
@@ -20,14 +22,15 @@
 from bring_api.types import BringItem, BringItemOperation, BringNotificationType
 
 from .conftest import (
     BRING_GET_ALL_ITEM_DETAILS_RESPONSE,
     BRING_GET_LIST_RESPONSE,
     BRING_LOAD_LISTS_RESPONSE,
     BRING_LOGIN_RESPONSE,
+    BRING_TOKEN_RESPONSE,
     BRING_USER_ACCOUNT_RESPONSE,
     BRING_USER_SETTINGS_RESPONSE,
     UUID,
 )
 
 load_dotenv()
 
@@ -50,30 +53,34 @@
         """Test does_user_exist for unknown user."""
         mocked.get("https://api.getbring.com/rest/bringusers?email=EMAIL", status=404)
         with pytest.raises(BringUserUnknownException):
             await bring.does_user_exist("EMAIL")
 
     async def test_mail_value_error(self, mocked, bring, monkeypatch):
         """Test does_user_exist for unknown user."""
-        mocked.get("https://api.getbring.com/rest/bringusers?email=", status=200)
+        mocked.get(
+            "https://api.getbring.com/rest/bringusers?email=", status=HTTPStatus.OK
+        )
         monkeypatch.setattr(bring, "mail", None)
 
         with pytest.raises(ValueError, match="Argument mail missing."):
             await bring.does_user_exist()
 
     async def test_user_exist_with_parameter(self, mocked, bring):
         """Test does_user_exist for known user."""
-        mocked.get("https://api.getbring.com/rest/bringusers?email=EMAIL", status=200)
+        mocked.get(
+            "https://api.getbring.com/rest/bringusers?email=EMAIL", status=HTTPStatus.OK
+        )
         assert await bring.does_user_exist("EMAIL") is True
 
     async def test_user_exist_without_parameter(self, mocked, bring):
         """Test does_user_exist for known user."""
         mocked.get(
             "https://api.getbring.com/rest/bringusers?email=EMAIL",
-            status=200,
+            status=HTTPStatus.OK,
         )
         assert await bring.does_user_exist() is True
 
     @pytest.mark.parametrize(
         ("exception", "expected"),
         [
             (asyncio.TimeoutError, BringRequestException),
@@ -105,22 +112,22 @@
         with pytest.raises(BringAuthException, match=expected):
             await bring.login()
 
     async def test_unauthorized(self, mocked, bring):
         """Test login with unauthorized user."""
         mocked.post(
             "https://api.getbring.com/rest/v2/bringauth",
-            status=401,
+            status=HTTPStatus.UNAUTHORIZED,
             payload={"message": ""},
         )
         expected = "Login failed due to authorization failure, please check your email and password."
         with pytest.raises(BringAuthException, match=expected):
             await bring.login()
 
-    @pytest.mark.parametrize("status", [200, 401])
+    @pytest.mark.parametrize("status", [HTTPStatus.OK, HTTPStatus.UNAUTHORIZED])
     async def test_parse_exception(self, mocked, bring, status):
         """Test parse exceptions."""
         mocked.post(
             "https://api.getbring.com/rest/v2/bringauth",
             status=status,
             body="not json",
             content_type="application/json",
@@ -143,15 +150,15 @@
             await bring.login()
 
     async def test_login(self, mocked, bring, monkeypatch):
         """Test login with valid user."""
 
         mocked.post(
             "https://api.getbring.com/rest/v2/bringauth",
-            status=200,
+            status=HTTPStatus.OK,
             payload=BRING_LOGIN_RESPONSE,
         )
 
         async def mocked_get_user_account(*args, **kwargs):
             """Mock get_user_account."""
             return {"userLocale": {"language": "de", "country": "DE"}}
 
@@ -186,36 +193,48 @@
     """Tests for load_lists method."""
 
     async def test_load_lists(self, bring, mocked, monkeypatch):
         """Test load_lists."""
 
         mocked.get(
             f"https://api.getbring.com/rest/bringusers/{UUID}/lists",
-            status=200,
+            status=HTTPStatus.OK,
             payload=BRING_LOAD_LISTS_RESPONSE,
         )
         monkeypatch.setattr(bring, "uuid", UUID)
 
         lists = await bring.load_lists()
 
         assert lists == BRING_LOAD_LISTS_RESPONSE
 
-    async def test_parse_exception(self, mocked, bring, monkeypatch):
+    @pytest.mark.parametrize("status", [HTTPStatus.OK, HTTPStatus.UNAUTHORIZED])
+    async def test_parse_exception(self, mocked, bring, monkeypatch, status):
         """Test parse exceptions."""
         mocked.get(
             f"https://api.getbring.com/rest/bringusers/{UUID}/lists",
-            status=200,
+            status=status,
             body="not json",
             content_type="application/json",
         )
         monkeypatch.setattr(bring, "uuid", UUID)
 
         with pytest.raises(BringParseException):
             await bring.load_lists()
 
+    async def test_unauthorized(self, mocked, bring, monkeypatch):
+        """Test unauthorized exception."""
+        mocked.get(
+            f"https://api.getbring.com/rest/bringusers/{UUID}/lists",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+        monkeypatch.setattr(bring, "uuid", UUID)
+        with pytest.raises(BringAuthException):
+            await bring.load_lists()
+
     @pytest.mark.parametrize(
         "exception",
         [
             asyncio.TimeoutError,
             aiohttp.ClientError,
         ],
     )
@@ -250,24 +269,24 @@
         item_name: str,
         mocked,
     ):
         """Test GOING_SHOPPING notification."""
 
         mocked.post(
             f"https://api.getbring.com/rest/v2/bringnotifications/lists/{UUID}",
-            status=200,
+            status=HTTPStatus.OK,
         )
         resp = await bring.notify(UUID, notification_type, item_name)
-        assert resp.status == 200
+        assert resp.status == HTTPStatus.OK
 
     async def test_notify_urgent_message_item_name_missing(self, bring, mocked):
         """Test URGENT_MESSAGE notification."""
         mocked.post(
             f"https://api.getbring.com/rest/v2/bringnotifications/lists/{UUID}",
-            status=200,
+            status=HTTPStatus.OK,
         )
         with pytest.raises(
             ValueError,
             match="notificationType is URGENT_MESSAGE but argument itemName missing.",
         ):
             await bring.notify(UUID, BringNotificationType.URGENT_MESSAGE, "")
 
@@ -308,14 +327,36 @@
             f"https://api.getbring.com/rest/v2/bringnotifications/lists/{UUID}",
             exception=exception,
         )
 
         with pytest.raises(BringRequestException):
             await bring.notify(UUID, BringNotificationType.GOING_SHOPPING)
 
+    async def test_unauthorized(self, mocked, bring):
+        """Test unauthorized exception."""
+        mocked.post(
+            f"https://api.getbring.com/rest/v2/bringnotifications/lists/{UUID}",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+        with pytest.raises(BringAuthException):
+            await bring.notify(UUID, BringNotificationType.GOING_SHOPPING)
+
+    async def test_parse_exception(self, mocked, bring):
+        """Test parse exceptions."""
+        mocked.post(
+            f"https://api.getbring.com/rest/v2/bringnotifications/lists/{UUID}",
+            status=HTTPStatus.UNAUTHORIZED,
+            body="not json",
+            content_type="application/json",
+        )
+
+        with pytest.raises(BringParseException):
+            await bring.notify(UUID, BringNotificationType.GOING_SHOPPING)
+
 
 class TestGetList:
     """Tests for get_list method."""
 
     @pytest.mark.parametrize(
         "exception",
         [
@@ -330,32 +371,43 @@
             f"https://api.getbring.com/rest/v2/bringlists/{UUID}",
             exception=exception,
         )
 
         with pytest.raises(BringRequestException):
             await bring.get_list(UUID)
 
-    async def test_parse_exception(self, mocked, bring, monkeypatch):
+    async def test_unauthorized(self, mocked, bring):
+        """Test unauthorized exception."""
+        mocked.get(
+            f"https://api.getbring.com/rest/v2/bringlists/{UUID}",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+        with pytest.raises(BringAuthException):
+            await bring.get_list(UUID)
+
+    @pytest.mark.parametrize("status", [HTTPStatus.OK, HTTPStatus.UNAUTHORIZED])
+    async def test_parse_exception(self, mocked, bring, monkeypatch, status):
         """Test parse exceptions."""
         mocked.get(
             f"https://api.getbring.com/rest/v2/bringlists/{UUID}",
-            status=200,
+            status=status,
             body="not json",
             content_type="application/json",
         )
         monkeypatch.setattr(bring, "uuid", UUID)
 
         with pytest.raises(BringParseException):
             await bring.get_list(UUID)
 
     async def test_get_list(self, mocked, bring, monkeypatch):
         """Test get list."""
         mocked.get(
             f"https://api.getbring.com/rest/v2/bringlists/{UUID}",
-            status=200,
+            status=HTTPStatus.OK,
             payload=BRING_GET_LIST_RESPONSE,
         )
 
         monkeypatch.setattr(Bring, "_Bring__locale", lambda _, x: "de-DE")
         monkeypatch.setattr(Bring, "_Bring__translate", mocked_translate)
         monkeypatch.setattr(bring, "uuid", UUID)
 
@@ -366,15 +418,15 @@
 class TestGetAllItemDetails:
     """Test for get_all_item_details method."""
 
     async def test_get_all_item_details(self, mocked, bring):
         """Test get_all_item_details."""
         mocked.get(
             f"https://api.getbring.com/rest/bringlists/{UUID}/details",
-            status=200,
+            status=HTTPStatus.OK,
             payload=BRING_GET_ALL_ITEM_DETAILS_RESPONSE,
         )
 
         data = await bring.get_all_item_details(UUID)
         assert data == BRING_GET_ALL_ITEM_DETAILS_RESPONSE
 
     async def test_list_not_found(self, mocked, bring):
@@ -384,19 +436,30 @@
             status=404,
             reason=f"List with uuid '{UUID}' not found",
         )
 
         with pytest.raises(BringRequestException):
             await bring.get_all_item_details(UUID)
 
-    async def test_parse_exception(self, mocked, bring):
+    async def test_unauthorized(self, mocked, bring):
+        """Test unauthorized exception."""
+        mocked.get(
+            f"https://api.getbring.com/rest/bringlists/{UUID}/details",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+        with pytest.raises(BringAuthException):
+            await bring.get_all_item_details(UUID)
+
+    @pytest.mark.parametrize("status", [HTTPStatus.OK, HTTPStatus.UNAUTHORIZED])
+    async def test_parse_exception(self, mocked, bring, status):
         """Test parse exceptions."""
         mocked.get(
             f"https://api.getbring.com/rest/bringlists/{UUID}/details",
-            status=200,
+            status=status,
             body="not json",
             content_type="application/json",
         )
 
         with pytest.raises(BringParseException):
             await bring.get_all_item_details(UUID)
 
@@ -728,15 +791,15 @@
         assert len(dictionaries) == 19  # de-CH is skipped
 
     async def test_load_fallback_to_download(self, bring, mocked, monkeypatch):
         """Test loading json and fallback to download from web."""
         mocked.get(
             "https://web.getbring.com/locale/articles.de-DE.json",
             payload={"test": "test"},
-            status=200,
+            status=HTTPStatus.OK,
         )
 
         monkeypatch.setattr(bring, "user_locale", "de-DE")
 
         monkeypatch.setattr(
             Bring,
             "_Bring__load_article_translations_from_file",
@@ -770,15 +833,15 @@
         with pytest.raises(BringRequestException):
             await bring._Bring__load_article_translations()
 
     async def test_parse_exception(self, bring, mocked, monkeypatch):
         """Test loading json and fallback to download from web."""
         mocked.get(
             "https://web.getbring.com/locale/articles.de-DE.json",
-            status=200,
+            status=HTTPStatus.OK,
             body="not json",
             content_type="application/json",
         )
 
         monkeypatch.setattr(bring, "user_locale", "de-DE")
 
         monkeypatch.setattr(
@@ -795,15 +858,15 @@
 
     async def test_get_user_account(self, bring, mocked, monkeypatch):
         """Test for get_user_account."""
 
         mocked.get(
             f"https://api.getbring.com/rest/v2/bringusers/{UUID}",
             payload=BRING_USER_ACCOUNT_RESPONSE,
-            status=200,
+            status=HTTPStatus.OK,
         )
 
         monkeypatch.setattr(bring, "uuid", UUID)
         data = await bring.get_user_account()
 
         assert data == BRING_USER_ACCOUNT_RESPONSE
 
@@ -822,19 +885,31 @@
             exception=exception,
         )
         monkeypatch.setattr(bring, "uuid", UUID)
 
         with pytest.raises(BringRequestException):
             await bring.get_user_account()
 
-    async def test_parse_exception(self, mocked, bring, monkeypatch):
+    async def test_unauthorized(self, mocked, bring, monkeypatch):
+        """Test unauthorized exception."""
+        mocked.get(
+            f"https://api.getbring.com/rest/v2/bringusers/{UUID}",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+        monkeypatch.setattr(bring, "uuid", UUID)
+        with pytest.raises(BringAuthException):
+            await bring.get_user_account()
+
+    @pytest.mark.parametrize("status", [HTTPStatus.OK, HTTPStatus.UNAUTHORIZED])
+    async def test_parse_exception(self, mocked, bring, monkeypatch, status):
         """Test parse exceptions."""
         mocked.get(
             f"https://api.getbring.com/rest/v2/bringusers/{UUID}",
-            status=200,
+            status=status,
             body="not json",
             content_type="application/json",
         )
         monkeypatch.setattr(bring, "uuid", UUID)
 
         with pytest.raises(BringParseException):
             await bring.get_user_account()
@@ -845,15 +920,15 @@
 
     async def test_get_all_user_settings(self, bring, mocked, monkeypatch):
         """Test for get_user_account."""
 
         mocked.get(
             f"https://api.getbring.com/rest/bringusersettings/{UUID}",
             payload=BRING_USER_SETTINGS_RESPONSE,
-            status=200,
+            status=HTTPStatus.OK,
         )
 
         monkeypatch.setattr(bring, "uuid", UUID)
         data = await bring.get_all_user_settings()
 
         assert data == BRING_USER_SETTINGS_RESPONSE
 
@@ -872,19 +947,31 @@
             exception=exception,
         )
         monkeypatch.setattr(bring, "uuid", UUID)
 
         with pytest.raises(BringRequestException):
             await bring.get_all_user_settings()
 
-    async def test_parse_exception(self, mocked, bring, monkeypatch):
+    async def test_unauthorized(self, mocked, bring, monkeypatch):
+        """Test unauthorized exception."""
+        mocked.get(
+            f"https://api.getbring.com/rest/bringusersettings/{UUID}",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+        monkeypatch.setattr(bring, "uuid", UUID)
+        with pytest.raises(BringAuthException):
+            await bring.get_all_user_settings()
+
+    @pytest.mark.parametrize("status", [HTTPStatus.OK, HTTPStatus.UNAUTHORIZED])
+    async def test_parse_exception(self, mocked, bring, monkeypatch, status):
         """Test parse exceptions."""
         mocked.get(
             f"https://api.getbring.com/rest/bringusersettings/{UUID}",
-            status=200,
+            status=status,
             body="not json",
             content_type="application/json",
         )
         monkeypatch.setattr(bring, "uuid", UUID)
 
         with pytest.raises(BringParseException):
             await bring.get_all_user_settings()
@@ -1097,24 +1184,24 @@
                     ),
                 }
             ],
             "sender": "",
         }
         mocked.put(
             url := f"https://api.getbring.com/rest/v2/bringlists/{UUID}/items",
-            status=200,
+            status=HTTPStatus.OK,
         )
         monkeypatch.setattr(Bring, "_Bring__locale", lambda _, x: "de-DE")
         monkeypatch.setattr(Bring, "_Bring__translate", mocked_translate)
 
         if operation:
             r = await bring.batch_update_list(UUID, item, operation)
         else:
             r = await bring.batch_update_list(UUID, item)
-        assert r.status == 200
+        assert r.status == HTTPStatus.OK
         mocked.assert_called_with(
             url,
             method="PUT",
             headers=DEFAULT_HEADERS,
             data=None,
             json=expected,
         )
@@ -1175,22 +1262,22 @@
                     "operation": "REMOVE",
                 },
             ],
             "sender": "",
         }
         mocked.put(
             url := f"https://api.getbring.com/rest/v2/bringlists/{UUID}/items",
-            status=200,
+            status=HTTPStatus.OK,
         )
         monkeypatch.setattr(Bring, "_Bring__locale", lambda _, x: "de-DE")
         monkeypatch.setattr(Bring, "_Bring__translate", mocked_translate)
 
         r = await bring.batch_update_list(UUID, test_items)
 
-        assert r.status == 200
+        assert r.status == HTTPStatus.OK
         mocked.assert_called_with(
             url,
             method="PUT",
             headers=DEFAULT_HEADERS,
             data=None,
             json=expected,
         )
@@ -1210,7 +1297,97 @@
             exception=exception,
         )
 
         with pytest.raises(BringRequestException):
             await bring.batch_update_list(
                 UUID, BringItem(itemId="item_name", spec="spec", uuid=UUID)
             )
+
+    async def test_unauthorized(self, mocked, bring, monkeypatch):
+        """Test unauthorized exception."""
+        mocked.put(
+            f"https://api.getbring.com/rest/v2/bringlists/{UUID}/items",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+
+        with pytest.raises(BringAuthException):
+            await bring.batch_update_list(
+                UUID, BringItem(itemId="item_name", spec="spec", uuid=UUID)
+            )
+
+    async def test_parse_exception(self, mocked, bring, monkeypatch):
+        """Test parse exceptions."""
+        mocked.put(
+            f"https://api.getbring.com/rest/v2/bringlists/{UUID}/items",
+            status=HTTPStatus.UNAUTHORIZED,
+            body="not json",
+            content_type="application/json",
+        )
+
+        with pytest.raises(BringParseException):
+            await bring.batch_update_list(
+                UUID, BringItem(itemId="item_name", spec="spec", uuid=UUID)
+            )
+
+
+class TestRetrieveNewAccessToken:
+    """Test for retrieve_new_access_token method."""
+
+    async def test_retrieve_new_access_token(self, mocked, bring, monkeypatch):
+        """Test retrieve_new_access_token."""
+        mocked.post(
+            "https://api.getbring.com/rest/v2/bringauth/token",
+            status=HTTPStatus.OK,
+            payload=BRING_TOKEN_RESPONSE,
+        )
+        monkeypatch.setattr(bring, "refresh_token", "test_refresh_token")
+        monkeypatch.setattr(time, "time", lambda: 0)
+        data = await bring.retrieve_new_access_token()
+
+        assert data == BRING_TOKEN_RESPONSE
+        assert bring.headers["Authorization"] == "Bearer {access_token}"
+        assert bring.expires_in == BRING_TOKEN_RESPONSE["expires_in"]
+
+    @pytest.mark.parametrize(
+        "exception",
+        [
+            asyncio.TimeoutError,
+            aiohttp.ClientError,
+        ],
+    )
+    async def test_request_exception(self, mocked, bring, exception):
+        """Test request exceptions."""
+
+        mocked.post(
+            "https://api.getbring.com/rest/v2/bringauth/token",
+            exception=exception,
+        )
+
+        with pytest.raises(BringRequestException):
+            await bring.retrieve_new_access_token()
+
+    async def test_auth_exception(self, mocked, bring):
+        """Test request exceptions."""
+
+        mocked.post(
+            "https://api.getbring.com/rest/v2/bringauth/token",
+            status=HTTPStatus.UNAUTHORIZED,
+            payload={"message": ""},
+        )
+
+        with pytest.raises(BringAuthException):
+            await bring.retrieve_new_access_token()
+
+    @pytest.mark.parametrize("status", [HTTPStatus.OK, HTTPStatus.UNAUTHORIZED])
+    async def test_parse_exception(self, mocked, bring, status):
+        """Test request exceptions."""
+
+        mocked.post(
+            "https://api.getbring.com/rest/v2/bringauth/token",
+            status=status,
+            body="not json",
+            content_type="application/json",
+        )
+
+        with pytest.raises(BringParseException):
+            await bring.retrieve_new_access_token()
```

