# Comparing `tmp/gpsoauth-1.0.4.tar.gz` & `tmp/gpsoauth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpsoauth-1.0.4.tar", max compression
+gzip compressed data, was "gpsoauth-1.1.0.tar", max compression
```

## Comparing `gpsoauth-1.0.4.tar` & `gpsoauth-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2021-04-06 14:55:06.790788 gpsoauth-1.0.4/LICENSE
--rw-r--r--   0        0        0     2168 2023-06-02 00:53:26.640231 gpsoauth-1.0.4/README.md
--rw-r--r--   0        0        0     5731 2023-11-28 20:18:13.255418 gpsoauth-1.0.4/gpsoauth/__init__.py
--rw-r--r--   0        0        0     1618 2021-04-06 14:55:06.790788 gpsoauth-1.0.4/gpsoauth/google.py
--rw-r--r--   0        0        0        0 2021-04-06 14:55:06.790788 gpsoauth-1.0.4/gpsoauth/py.typed
--rw-r--r--   0        0        0     1053 2021-04-06 14:55:06.790788 gpsoauth-1.0.4/gpsoauth/util.py
--rw-r--r--   0        0        0     1677 2023-11-28 20:20:13.535407 gpsoauth-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 gpsoauth-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-04-06 14:55:06.790788 gpsoauth-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2865 2024-04-10 13:54:32.972407 gpsoauth-1.1.0/README.md
+-rw-r--r--   0        0        0     7220 2024-04-10 13:54:32.972407 gpsoauth-1.1.0/gpsoauth/__init__.py
+-rw-r--r--   0        0        0     1618 2021-04-06 14:55:06.790788 gpsoauth-1.1.0/gpsoauth/google.py
+-rw-r--r--   0        0        0        0 2021-04-06 14:55:06.790788 gpsoauth-1.1.0/gpsoauth/py.typed
+-rw-r--r--   0        0        0     1053 2021-04-06 14:55:06.790788 gpsoauth-1.1.0/gpsoauth/util.py
+-rw-r--r--   0        0        0     1677 2024-04-10 13:58:20.522370 gpsoauth-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3908 1970-01-01 00:00:00.000000 gpsoauth-1.1.0/PKG-INFO
```

### Comparing `gpsoauth-1.0.4/LICENSE` & `gpsoauth-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpsoauth-1.0.4/README.md` & `gpsoauth-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,18 +30,43 @@
 [gmusicapi does here](https://github.com/simon-weber/gmusicapi/blob/87a802ab3a59a7fa2974fd9755d59a55275484d9/gmusicapi/session.py#L267-L278).
 
 Many thanks to Dima Kovalenko for reverse engineering the EncryptedPasswd signature in
 <https://web.archive.org/web/20150814054004/http://codedigging.com/blog/2014-06-09-about-encryptedpasswd/>.
 
 For an explanation of recent changes, see [the changelog](https://github.com/simon-weber/gpsoauth/blob/master/CHANGELOG.md).
 
+## Alternative flow
+
+There is an alternative login flow if you are experiencing `BadAuthentication` errors.
+
+1. Login to your Google account (Ex: Via https://accounts.google.com/EmbeddedSetup)
+2. Obtain the value of the `oauth_token` cookie
+3. Perform the token exchange:
+
+```python
+import gpsoauth
+
+email = 'example@gmail.com'
+android_id = '0123456789abcdef'
+token = '...' # insert the oauth_token here
+
+master_response = gpsoauth.exchange_token(email, token, android_id)
+master_token = master_response['Token']
+
+auth_response = gpsoauth.perform_oauth(
+    email, master_token, android_id,
+    service='sj', app='com.google.android.music',
+    client_sig='...')
+token = auth_response['Auth']
+```
+
 ## Ports
 
 - C\#: <https://github.com/vemacs/GPSOAuthSharp>
 - Ruby: <https://github.com/bryanmytko/gpsoauth>
 - Java: <https://github.com/svarzee/gpsoauth-java>
 - C++: <https://github.com/dvirtz/gpsoauth-cpp> and <https://github.com/Iciclelz/gpsoauthclient>
 
 ## Contributing
 
 See [Contributing guidelines](https://github.com/simon-weber/gpsoauth/blob/master/CONTRIBUTING.md).
-This is an open-source project and all countributions are highly welcomed.
+This is an open-source project and all contributions are highly welcomed.
```

### Comparing `gpsoauth-1.0.4/gpsoauth/__init__.py` & `gpsoauth-1.1.0/gpsoauth/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -151,14 +151,68 @@
         "callerSig": client_sig,
         "droidguard_results": "dummy123",
     }
 
     return _perform_auth_request(data, proxy)
 
 
+def exchange_token(
+    email: str,
+    token: str,
+    android_id: str,
+    service: str = "ac2dm",
+    device_country: str = "us",
+    operator_country: str = "us",
+    lang: str = "en",
+    sdk_version: int = 17,
+    proxy: MutableMapping[str, str] | None = None,
+    client_sig: str = "38918a453d07199354f8b19af05ec6562ced5788",
+) -> dict[str, str]:
+    """
+    Exchanges a web oauth_token for a master token.
+
+    Return a dict, eg::
+        {
+            'Auth': '...',
+            'Email': 'email@gmail.com',
+            'GooglePlusUpgrade': '1',
+            'LSID': '...',
+            'PicasaUser': 'My Name',
+            'RopRevision': '1',
+            'RopText': ' ',
+            'SID': '...',
+            'Token': 'oauth2rt_1/...',
+            'firstName': 'My',
+            'lastName': 'Name',
+            'services': 'hist,mail,googleme,...'
+        }
+    """
+
+    data: dict[str, int | str | bytes] = {
+        "accountType": "HOSTED_OR_GOOGLE",
+        "Email": email,
+        "has_permission": 1,
+        "add_account": 1,
+        "ACCESS_TOKEN": 1,
+        "Token": token,
+        "service": service,
+        "source": "android",
+        "androidId": android_id,
+        "device_country": device_country,
+        "operatorCountry": operator_country,
+        "lang": lang,
+        "sdk_version": sdk_version,
+        "client_sig": client_sig,
+        "callerSig": client_sig,
+        "droidguard_results": "dummy123",
+    }
+
+    return _perform_auth_request(data, proxy)
+
+
 def perform_oauth(
     email: str,
     master_token: str,
     android_id: str,
     service: str,
     app: str,
     client_sig: str,
```

### Comparing `gpsoauth-1.0.4/gpsoauth/google.py` & `gpsoauth-1.1.0/gpsoauth/google.py`

 * *Files identical despite different names*

### Comparing `gpsoauth-1.0.4/gpsoauth/util.py` & `gpsoauth-1.1.0/gpsoauth/util.py`

 * *Files identical despite different names*

### Comparing `gpsoauth-1.0.4/pyproject.toml` & `gpsoauth-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpsoauth"
-version = "1.0.4"
+version = "1.1.0"
 description = "A python client library for Google Play Services OAuth."
 authors = ["Simon Weber <simon@simonmweber.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `gpsoauth-1.0.4/PKG-INFO` & `gpsoauth-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpsoauth
-Version: 1.0.4
+Version: 1.1.0
 Summary: A python client library for Google Play Services OAuth.
 Home-page: https://github.com/simon-weber/gpsoauth
 License: MIT
 Author: Simon Weber
 Author-email: simon@simonmweber.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,19 +57,44 @@
 [gmusicapi does here](https://github.com/simon-weber/gmusicapi/blob/87a802ab3a59a7fa2974fd9755d59a55275484d9/gmusicapi/session.py#L267-L278).
 
 Many thanks to Dima Kovalenko for reverse engineering the EncryptedPasswd signature in
 <https://web.archive.org/web/20150814054004/http://codedigging.com/blog/2014-06-09-about-encryptedpasswd/>.
 
 For an explanation of recent changes, see [the changelog](https://github.com/simon-weber/gpsoauth/blob/master/CHANGELOG.md).
 
+## Alternative flow
+
+There is an alternative login flow if you are experiencing `BadAuthentication` errors.
+
+1. Login to your Google account (Ex: Via https://accounts.google.com/EmbeddedSetup)
+2. Obtain the value of the `oauth_token` cookie
+3. Perform the token exchange:
+
+```python
+import gpsoauth
+
+email = 'example@gmail.com'
+android_id = '0123456789abcdef'
+token = '...' # insert the oauth_token here
+
+master_response = gpsoauth.exchange_token(email, token, android_id)
+master_token = master_response['Token']
+
+auth_response = gpsoauth.perform_oauth(
+    email, master_token, android_id,
+    service='sj', app='com.google.android.music',
+    client_sig='...')
+token = auth_response['Auth']
+```
+
 ## Ports
 
 - C\#: <https://github.com/vemacs/GPSOAuthSharp>
 - Ruby: <https://github.com/bryanmytko/gpsoauth>
 - Java: <https://github.com/svarzee/gpsoauth-java>
 - C++: <https://github.com/dvirtz/gpsoauth-cpp> and <https://github.com/Iciclelz/gpsoauthclient>
 
 ## Contributing
 
 See [Contributing guidelines](https://github.com/simon-weber/gpsoauth/blob/master/CONTRIBUTING.md).
-This is an open-source project and all countributions are highly welcomed.
+This is an open-source project and all contributions are highly welcomed.
```

