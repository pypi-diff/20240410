# Comparing `tmp/reflex-google-recaptcha-v2-0.0.2.tar.gz` & `tmp/reflex-google-recaptcha-v2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-google-recaptcha-v2-0.0.2.tar", last modified: Thu Mar 21 18:56:40 2024, max compression
+gzip compressed data, was "reflex-google-recaptcha-v2-0.0.3.tar", last modified: Wed Apr 10 18:55:45 2024, max compression
```

## Comparing `reflex-google-recaptcha-v2-0.0.2.tar` & `reflex-google-recaptcha-v2-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:56:40.153806 reflex-google-recaptcha-v2-0.0.2/
--rw-r--r--   0 masen      (502) staff       (20)     1864 2024-03-21 18:56:40.153589 reflex-google-recaptcha-v2-0.0.2/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)     1326 2024-03-18 00:39:17.000000 reflex-google-recaptcha-v2-0.0.2/README.md
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:56:40.151596 reflex-google-recaptcha-v2-0.0.2/custom_components/
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:56:40.152285 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2/
--rw-r--r--   0 masen      (502) staff       (20)       35 2024-03-18 00:41:03.000000 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2/__init__.py
--rw-r--r--   0 masen      (502) staff       (20)     5323 2024-03-21 18:18:17.000000 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2/google_recaptcha_v2.py
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:56:40.153266 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2.egg-info/
--rw-r--r--   0 masen      (502) staff       (20)     1864 2024-03-21 18:56:40.000000 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2.egg-info/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)      488 2024-03-21 18:56:40.000000 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2.egg-info/SOURCES.txt
--rw-r--r--   0 masen      (502) staff       (20)        1 2024-03-21 18:56:40.000000 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2.egg-info/dependency_links.txt
--rw-r--r--   0 masen      (502) staff       (20)       33 2024-03-21 18:56:40.000000 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2.egg-info/requires.txt
--rw-r--r--   0 masen      (502) staff       (20)       27 2024-03-21 18:56:40.000000 reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2.egg-info/top_level.txt
--rw-r--r--   0 masen      (502) staff       (20)      730 2024-03-21 18:54:10.000000 reflex-google-recaptcha-v2-0.0.2/pyproject.toml
--rw-r--r--   0 masen      (502) staff       (20)       38 2024-03-21 18:56:40.153849 reflex-google-recaptcha-v2-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:55:45.673607 reflex-google-recaptcha-v2-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 18:55:45.669607 reflex-google-recaptcha-v2-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-10 18:55:05.000000 reflex-google-recaptcha-v2-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:55:45.669607 reflex-google-recaptcha-v2-0.0.3/custom_components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:55:45.669607 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-10 18:55:05.000000 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-10 18:55:05.000000 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2/google_recaptcha_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:55:45.669607 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 18:55:45.000000 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 18:55:45.000000 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:55:45.000000 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 18:55:45.000000 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 18:55:45.000000 reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-10 18:55:05.000000 reflex-google-recaptcha-v2-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:55:45.673607 reflex-google-recaptcha-v2-0.0.3/setup.cfg
```

### Comparing `reflex-google-recaptcha-v2-0.0.2/PKG-INFO` & `reflex-google-recaptcha-v2-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: reflex-google-recaptcha-v2
-Version: 0.0.2
-Summary: Reflex custom component google-recaptcha-v2
+Version: 0.0.3
+Summary: Google ReCAPTCHA v2 Integration
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-google-recaptcha-v2
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: httpx>=0.25.1
+Requires-Dist: reflex>=0.4.6
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # google-recaptcha-v2
 
 A Reflex custom component google-recaptcha-v2.
```

### Comparing `reflex-google-recaptcha-v2-0.0.2/README.md` & `reflex-google-recaptcha-v2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2/google_recaptcha_v2.py` & `reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2/google_recaptcha_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""Reflex custom component GoogleRecaptchaV2."""
+"""Google ReCAPTCHA v2 Integration"""
 
 from __future__ import annotations
 
 import os
-from typing import Any, Dict
 
 import httpx
 
 import reflex as rx
 
 
 VERIFY_ENDPOINT = "https://www.google.com/recaptcha/api/siteverify"
@@ -52,18 +51,14 @@
         return self._is_valid
 
 
 class GoogleRecaptchaV2(rx.NoSSRComponent):
     """GoogleRecaptchaV2 component.
 
     Event Triggers:
-        - async_script_on_load: optional callback when the google recaptcha script has been loaded
-        - on_change: The function to be called when the user successfully completes the captcha
-        - on_errored: optional callback when the challenge errored, most likely due to network issues.
-        - on_expired: optional callback when the challenge is expired and has to be redone by user. By default it will call the onChange with null to signify expired callback.
     """
 
     # The React library to wrap.
     library = "react-google-recaptcha"
 
     # The React component tag.
     tag = "ReCAPTCHA"
@@ -93,32 +88,35 @@
 
     # The type of initial captcha - image or audio (defaults: image).
     type: rx.Var[str]
 
     # The theme of the widget - light or dark (defaults: light).
     theme: rx.Var[str]
 
+    # The function to be called when the user successfully completes the captcha
+    on_change: rx.EventHandler[lambda e0: [e0]]
+
+    # Optional callback when the google recaptcha script has been loaded
+    async_script_on_load: rx.EventHandler[lambda e0: [e0]]
+
+    # Optional callback when the challenge errored, most likely due to network issues.
+    on_errored: rx.EventHandler[lambda e0: [e0]]
+
+    # Optional callback when the challenge is expired and has to be redone by user. By default it will call the onChange with null to signify expired callback.
+    on_expired: rx.EventHandler[lambda e0: [e0]]
+
     @classmethod
     def create(cls, **props) -> "GoogleRecaptchaV2":
         if props.get("size") == "invisible":
             props.setdefault("id", rx.vars.get_unique_variable_name())
             raise NotImplementedError("Invisible mode is not currently working.")
         props.setdefault("sitekey", SITE_KEY)
         props.setdefault("on_change", GoogleRecaptchaV2State.verify_captcha)
         return super().create(**props)
 
-    def get_event_triggers(self) -> Dict[str, Any]:
-        return {
-            **super().get_event_triggers(),
-            "async_script_on_load": lambda e0: [e0],
-            "on_change": lambda e0: [e0],
-            "on_errored": lambda e0: [e0],
-            "on_expired": lambda e0: [e0],
-        }
-
     def api(self) -> "GoogleRecaptchaV2API" | None:
         raise NotImplementedError("Invisible mode is not currently working.")
         ref = self.get_ref()
         if ref:
             return GoogleRecaptchaV2API(ref_name=self.get_ref())
         raise ValueError("Be sure to set an id on the component to use the API.")
```

### Comparing `reflex-google-recaptcha-v2-0.0.2/custom_components/reflex_google_recaptcha_v2.egg-info/PKG-INFO` & `reflex-google-recaptcha-v2-0.0.3/custom_components/reflex_google_recaptcha_v2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: reflex-google-recaptcha-v2
-Version: 0.0.2
-Summary: Reflex custom component google-recaptcha-v2
+Version: 0.0.3
+Summary: Google ReCAPTCHA v2 Integration
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-google-recaptcha-v2
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: httpx>=0.25.1
+Requires-Dist: reflex>=0.4.6
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # google-recaptcha-v2
 
 A Reflex custom component google-recaptcha-v2.
```

### Comparing `reflex-google-recaptcha-v2-0.0.2/pyproject.toml` & `reflex-google-recaptcha-v2-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,27 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-google-recaptcha-v2"
-version = "0.0.2"
-description = "Reflex custom component google-recaptcha-v2"
+version = "0.0.3"
+description = "Google ReCAPTCHA v2 Integration"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
 keywords = [
     "reflex",
     "reflex-custom-components"]
 
 dependencies = [
-    "reflex>=0.4.2"
+    "httpx>=0.25.1",
+    "reflex>=0.4.6",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
 ]
 
 [project.urls]
```

