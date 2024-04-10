# Comparing `tmp/lib2fas-0.1.6.tar.gz` & `tmp/lib2fas-0.1.7.tar.gz`

## Comparing `lib2fas-0.1.6.tar` & `lib2fas-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,44 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lib2fas-0.1.6/.env
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 lib2fas-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lib2fas-0.1.6/src/lib2fas/__about__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 lib2fas-0.1.6/src/lib2fas/__init__.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 lib2fas-0.1.6/src/lib2fas/_security.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 lib2fas-0.1.6/src/lib2fas/_types.py
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 lib2fas-0.1.6/src/lib2fas/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lib2fas-0.1.6/src/lib2fas/py.typed
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 lib2fas-0.1.6/src/lib2fas/utils.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/2fas-demo-minimal.2fas
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/2fas-demo-nopass.2fas
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/2fas-demo-pass.2fas
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/_shared.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/test_decrypted.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/test_encrypted.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 lib2fas-0.1.6/tests/test_other.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 lib2fas-0.1.6/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 lib2fas-0.1.6/LICENSE
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 lib2fas-0.1.6/README.md
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 lib2fas-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 lib2fas-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 lib2fas-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/.gitignore
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_55b65c9e5a43b9a2___about___py.html
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_55b65c9e5a43b9a2___init___py.html
+-rw-r--r--   0        0        0    45269 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_55b65c9e5a43b9a2__security_py.html
+-rw-r--r--   0        0        0    32631 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_55b65c9e5a43b9a2__types_py.html
+-rw-r--r--   0        0        0    45663 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_55b65c9e5a43b9a2_core_py.html
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_55b65c9e5a43b9a2_utils_py.html
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d___about___py.html
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d___init___py.html
+-rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d__security_py.html
+-rw-r--r--   0        0        0    24236 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d__types_py.html
+-rw-r--r--   0        0        0    86839 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d_cli_py.html
+-rw-r--r--   0        0        0    21656 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d_cli_settings_py.html
+-rw-r--r--   0        0        0    27737 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d_cli_support_py.html
+-rw-r--r--   0        0        0    45022 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d_core_py.html
+-rw-r--r--   0        0        0    10327 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d_main_py.html
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/d_ece9e2c2b8514e4d_utils_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/status.json
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 lib2fas-0.1.7/htmlcov/style.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lib2fas-0.1.7/src/lib2fas/__about__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 lib2fas-0.1.7/src/lib2fas/__init__.py
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 lib2fas-0.1.7/src/lib2fas/_security.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 lib2fas-0.1.7/src/lib2fas/_types.py
+-rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 lib2fas-0.1.7/src/lib2fas/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lib2fas-0.1.7/src/lib2fas/py.typed
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 lib2fas-0.1.7/src/lib2fas/utils.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/2fas-demo-minimal.2fas
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/2fas-demo-nopass.2fas
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/2fas-demo-pass.2fas
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/_shared.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/test_decrypted.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/test_encrypted.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 lib2fas-0.1.7/tests/test_other.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 lib2fas-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 lib2fas-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lib2fas-0.1.7/README.md
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 lib2fas-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 lib2fas-0.1.7/PKG-INFO
```

### Comparing `lib2fas-0.1.6/CHANGELOG.md` & `lib2fas-0.1.7/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.7 (2024-04-10)
+
+
+
+## v0.1.7 (2024-04-10)
+
+### Fix
+
+* Don't crash on missing (supported) keyring ([`2624e2a`](https://github.com/robinvandernoord/lib2fas-python/commit/2624e2a216adff37a76ab16e215d7829d5ffef64))
+
+### Documentation
+
+* Link to 2fas cli tool ([`791286c`](https://github.com/robinvandernoord/lib2fas-python/commit/791286c64652ccf935643e255d579cda08e0ad02))
+
+
 ## v0.1.6 (2024-03-01)
 
 ### Fix
 
 * Require the latest configuraptor, which includes a fix for 3.12 ([`bfae811`](https://github.com/robinvandernoord/lib2fas-python/commit/bfae811e0fdf46b0f9c80b823bbe020900740ed0))
 
 ## v0.1.5 (2024-02-29)
```

### Comparing `lib2fas-0.1.6/src/lib2fas/_security.py` & `lib2fas-0.1.7/src/lib2fas/_security.py`

 * *Files 19% similar despite different names*

```diff
@@ -68,15 +68,72 @@
     sha256.update(str(data).encode())
     return sha256.hexdigest()
 
 
 PREFIX = "2fas:"
 
 
-class KeyringManager:
+class KeyringManagerProtocol(typing.Protocol):
+    def retrieve_credentials(self, filename: str) -> Optional[str]:
+        """
+        Get the saved passphrase for a specific file.
+        """
+
+    def save_credentials(self, filename: str) -> str:
+        """
+        Query the user for a passphrase and store it in the keyring.
+        """
+
+    def delete_credentials(self, filename: str) -> None:
+        """
+        Remove a stored passphrase for a file.
+        """
+
+    def cleanup_keyring(self) -> None:
+        """
+        Remove all old items from the keyring.
+        """
+
+
+class DummyKeyringManager(KeyringManagerProtocol):
+    __cache: dict[str, str]
+
+    def __init__(self):
+        self.__cache = {}
+
+    def retrieve_credentials(self, filename: str) -> Optional[str]:
+        """
+        Get the saved passphrase for a specific file.
+        """
+        return self.__cache.get(filename, None)
+
+    def save_credentials(self, filename: str) -> str:
+        """
+        Query the user for a passphrase and store it in the keyring.
+        """
+        value = getpass.getpass(f"Passphrase for '{filename}'? ")
+        self.__cache[filename] = value
+        return value
+
+    def delete_credentials(self, filename: str) -> None:
+        """
+        Remove a stored passphrase for a file.
+        """
+        self.__cache.pop(filename, None)
+        return None
+
+    def cleanup_keyring(self) -> None:
+        """
+        Remove all old items from the keyring.
+        """
+        # self.__cache.clear() # disable to prevent double prompting
+        return None
+
+
+class KeyringManager(KeyringManagerProtocol):
     """
     Makes working with the keyring a bit easier.
 
     Stores passphrases for encrypted .2fas files in the keyring.
     When the user logs out, the keyring item is invalidated and the user is asked for the passphrase again.
     While the user stays logged in, the passphrase is then 'remembered'.
     """
@@ -86,14 +143,25 @@
 
     def __init__(self) -> None:
         """
         See _init.
         """
         self._init()
 
+    @classmethod
+    def or_dummy(cls) -> KeyringManagerProtocol:
+        """
+        Get a KeyringManager if keyring is available, or a DummyKeyringManger otherwise.
+        """
+        import keyring.backends.fail
+        if isinstance(keyring.get_keyring(), keyring.backends.fail.Keyring):
+            return DummyKeyringManager()
+
+        return cls()
+
     def _init(self) -> None:
         """
         Setup for a new instance.
 
         This is used instead of __init__ so you can call init again to set active appname (for pytest)
         """
         tmp_file = self.tmp_file
@@ -158,18 +226,18 @@
 
         collection = kr.get_preferred_collection()
 
         old = [
             item
             for item in collection.get_all_items()
             if (
-                service := item.get_attributes().get("service", "")
-            )  # must have a 'service' attribute, otherwise it's unrelated
-            and service.startswith(PREFIX)  # must be a 2fas: service, otherwise it's unrelated
-            and service != appname  # must not be the currently active session
+                   service := item.get_attributes().get("service", "")
+               )  # must have a 'service' attribute, otherwise it's unrelated
+               and service.startswith(PREFIX)  # must be a 2fas: service, otherwise it's unrelated
+               and service != appname  # must not be the currently active session
         ]
 
         for item in old:
             cls._delete_item(item)
 
         # get old 2fas: keyring items:
         return len(old)
@@ -177,8 +245,8 @@
     def cleanup_keyring(self) -> None:
         """
         Remove all old items from the keyring.
         """
         self._cleanup_keyring(self.appname)
 
 
-keyring_manager = KeyringManager()
+keyring_manager = KeyringManager.or_dummy()
```

### Comparing `lib2fas-0.1.6/src/lib2fas/_types.py` & `lib2fas-0.1.7/src/lib2fas/_types.py`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/src/lib2fas/core.py` & `lib2fas-0.1.7/src/lib2fas/core.py`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/tests/2fas-demo-minimal.2fas` & `lib2fas-0.1.7/tests/2fas-demo-minimal.2fas`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/tests/2fas-demo-nopass.2fas` & `lib2fas-0.1.7/tests/2fas-demo-nopass.2fas`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/tests/2fas-demo-pass.2fas` & `lib2fas-0.1.7/tests/2fas-demo-pass.2fas`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/tests/test_decrypted.py` & `lib2fas-0.1.7/tests/test_decrypted.py`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/tests/test_encrypted.py` & `lib2fas-0.1.7/tests/test_encrypted.py`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/LICENSE` & `lib2fas-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/README.md` & `lib2fas-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # lib2fas Python
 
 Unofficial implementation of 2fas for Python (as a library).
+This library serves as the backend for
+the [robinvandernoord/2fas-python](https://github.com/robinvandernoord/2fas-python) CLI, a command-line tool that
+provides an easy interface to interact with the 2fas TOTP.
 
 ## Installation
 
 To install this project, use pip:
 
 ```bash
 pip install lib2fas
@@ -15,32 +18,32 @@
 ## Usage
 
 After installing the package, you can import it in your Python scripts as follows:
 
 ```python
 import lib2fas
 
-services = lib2fas.load_services("/path/to/file.2fas", passphrase="optional") # -> TwoFactorStorage
+services = lib2fas.load_services("/path/to/file.2fas", passphrase="optional")  # -> TwoFactorStorage
 
-services.generate() # generate all TOTP keys
+services.generate()  # generate all TOTP keys
 
-gmail = services["gmail"] # exact match (case-insensitive), returns a list of 'TwoFactorAuthDetails' instances.
+gmail = services["gmail"]  # exact match (case-insensitive), returns a list of 'TwoFactorAuthDetails' instances.
 
-github = services.find("githbu") # fuzzy match should find GitHub, returns a new TwoFactorStorage.
+github = services.find("githbu")  # fuzzy match should find GitHub, returns a new TwoFactorStorage.
 
 for label, services in github.items():
     # one label can have multiple services!
-    for service in services: # 'service' is a TwoFactorAuthDetails instance
+    for service in services:  # 'service' is a TwoFactorAuthDetails instance
         # Print label, service name, and TOTP code
         print("Label:", label)
         print("Service Name:", service.name)
-        print("TOTP Code:", service.generate()) # or .generate_int() to get the code as a number.
+        print("TOTP Code:", service.generate())  # or .generate_int() to get the code as a number.
 ```
 
-The `passphrase` option of `load_services` is optional. 
+The `passphrase` option of `load_services` is optional.
 If you don't provide a password, but your file is encrypted, you will be prompted for the passphrase.
 If possible, this will be safely stored in the keychain manager of your OS* until the next reboot.
 
 * Note: only the "Secret Storage" keychain backend on Ubuntu Linux has been tested.
 
 ## License
```

### Comparing `lib2fas-0.1.6/pyproject.toml` & `lib2fas-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lib2fas-0.1.6/PKG-INFO` & `lib2fas-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib2fas
-Version: 0.1.6
+Version: 0.1.7
 Summary: Unofficial implementation of 2fas for Python (as a library)
 Project-URL: Documentation, https://github.com/robinvandernoord/lib2fas-python#readme
 Project-URL: Issues, https://github.com/robinvandernoord/lib2fas-python/issues
 Project-URL: Source, https://github.com/robinvandernoord/lib2fas-python
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -29,14 +29,17 @@
 Requires-Dist: python-semantic-release<8; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # lib2fas Python
 
 Unofficial implementation of 2fas for Python (as a library).
+This library serves as the backend for
+the [robinvandernoord/2fas-python](https://github.com/robinvandernoord/2fas-python) CLI, a command-line tool that
+provides an easy interface to interact with the 2fas TOTP.
 
 ## Installation
 
 To install this project, use pip:
 
 ```bash
 pip install lib2fas
@@ -47,32 +50,32 @@
 ## Usage
 
 After installing the package, you can import it in your Python scripts as follows:
 
 ```python
 import lib2fas
 
-services = lib2fas.load_services("/path/to/file.2fas", passphrase="optional") # -> TwoFactorStorage
+services = lib2fas.load_services("/path/to/file.2fas", passphrase="optional")  # -> TwoFactorStorage
 
-services.generate() # generate all TOTP keys
+services.generate()  # generate all TOTP keys
 
-gmail = services["gmail"] # exact match (case-insensitive), returns a list of 'TwoFactorAuthDetails' instances.
+gmail = services["gmail"]  # exact match (case-insensitive), returns a list of 'TwoFactorAuthDetails' instances.
 
-github = services.find("githbu") # fuzzy match should find GitHub, returns a new TwoFactorStorage.
+github = services.find("githbu")  # fuzzy match should find GitHub, returns a new TwoFactorStorage.
 
 for label, services in github.items():
     # one label can have multiple services!
-    for service in services: # 'service' is a TwoFactorAuthDetails instance
+    for service in services:  # 'service' is a TwoFactorAuthDetails instance
         # Print label, service name, and TOTP code
         print("Label:", label)
         print("Service Name:", service.name)
-        print("TOTP Code:", service.generate()) # or .generate_int() to get the code as a number.
+        print("TOTP Code:", service.generate())  # or .generate_int() to get the code as a number.
 ```
 
-The `passphrase` option of `load_services` is optional. 
+The `passphrase` option of `load_services` is optional.
 If you don't provide a password, but your file is encrypted, you will be prompted for the passphrase.
 If possible, this will be safely stored in the keychain manager of your OS* until the next reboot.
 
 * Note: only the "Secret Storage" keychain backend on Ubuntu Linux has been tested.
 
 ## License
```

