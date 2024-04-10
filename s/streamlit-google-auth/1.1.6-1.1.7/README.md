# Comparing `tmp/streamlit-google-auth-1.1.6.tar.gz` & `tmp/streamlit-google-auth-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-google-auth-1.1.6.tar", last modified: Wed Apr 10 08:27:47 2024, max compression
+gzip compressed data, was "streamlit-google-auth-1.1.7.tar", last modified: Wed Apr 10 08:40:24 2024, max compression
```

## Comparing `streamlit-google-auth-1.1.6.tar` & `streamlit-google-auth-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.200280 streamlit-google-auth-1.1.6/
--rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.6/LICENSE
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:27:47.200055 streamlit-google-auth-1.1.6/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.6/README.md
--rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 08:27:43.000000 streamlit-google-auth-1.1.6/pyproject.toml
--rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 08:27:47.200323 streamlit-google-auth-1.1.6/setup.cfg
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.198235 streamlit-google-auth-1.1.6/src/
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.198754 streamlit-google-auth-1.1.6/src/streamlit_google_auth/
--rw-r--r--   0 adrien     (501) staff       (20)     5320 2024-04-10 08:27:28.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.199477 streamlit-google-auth-1.1.6/src/streamlit_google_auth/cookie/
--rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth/cookie/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.199825 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/requires.txt
--rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/top_level.txt
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:40:24.908563 streamlit-google-auth-1.1.7/
+-rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.7/LICENSE
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:40:24.908313 streamlit-google-auth-1.1.7/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.7/README.md
+-rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 08:40:21.000000 streamlit-google-auth-1.1.7/pyproject.toml
+-rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 08:40:24.908610 streamlit-google-auth-1.1.7/setup.cfg
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:40:24.906200 streamlit-google-auth-1.1.7/src/
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:40:24.906741 streamlit-google-auth-1.1.7/src/streamlit_google_auth/
+-rw-r--r--   0 adrien     (501) staff       (20)     5356 2024-04-10 08:40:16.000000 streamlit-google-auth-1.1.7/src/streamlit_google_auth/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:40:24.907645 streamlit-google-auth-1.1.7/src/streamlit_google_auth/cookie/
+-rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.7/src/streamlit_google_auth/cookie/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:40:24.908049 streamlit-google-auth-1.1.7/src/streamlit_google_auth.egg-info/
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:40:24.000000 streamlit-google-auth-1.1.7/src/streamlit_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 08:40:24.000000 streamlit-google-auth-1.1.7/src/streamlit_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 08:40:24.000000 streamlit-google-auth-1.1.7/src/streamlit_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 08:40:24.000000 streamlit-google-auth-1.1.7/src/streamlit_google_auth.egg-info/requires.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 08:40:24.000000 streamlit-google-auth-1.1.7/src/streamlit_google_auth.egg-info/top_level.txt
```

### Comparing `streamlit-google-auth-1.1.6/LICENSE` & `streamlit-google-auth-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.6/PKG-INFO` & `streamlit-google-auth-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.6
+Version: 1.1.7
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit-google-auth-1.1.6/README.md` & `streamlit-google-auth-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.6/pyproject.toml` & `streamlit-google-auth-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit-google-auth"
-version = "1.1.6"
+version = "1.1.7"
 description = "Use Google authentification in streamlit"
 readme = "README.md"
 authors = [{ name = "Adrien Bouvais", email = "adrien.bouvais.pro@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `streamlit-google-auth-1.1.6/src/streamlit_google_auth/__init__.py` & `streamlit-google-auth-1.1.7/src/streamlit_google_auth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import google_auth_oauthlib.flow
 from googleapiclient.discovery import build
 
 from .cookie import CookieHandler
 
 class Authenticate:
     def __init__(self, secret_credentials_path:str, redirect_uri: str, cookie_name: str, cookie_key: str, cookie_expiry_days: float=30.0):
-        st.session_state['connected'] = False
+        st.session_state['connected']   =   st.session_state.get('connected', False) 
         self.secret_credentials_path    =   secret_credentials_path
         self.redirect_uri               =   redirect_uri
         self.cookie_handler             =   CookieHandler(cookie_name,
                                                           cookie_key,
                                                           cookie_expiry_days)
         
     def get_authorization_url(self) -> str:
@@ -56,28 +56,27 @@
 
             st.markdown(html_content, unsafe_allow_html=True)
 
     def check_authentification(self):
         if not st.session_state['connected']:
             token = self.cookie_handler.get_cookie()
             if token:
+                print("Token found")
                 user_info = {
                     'name': token['name'],
                     'email': token['email'],
                     'picture': token['picture'],
                     'id': token['oauth_id']
                 }
                 st.query_params.clear()
                 st.session_state["connected"] = True
                 st.session_state["user_info"] = user_info
                 st.session_state["oauth_id"] = user_info.get("id")
                 return
             
-            time.sleep(0.3)
-            
             if not st.session_state['connected']:
                 auth_code = st.query_params.get("code")
                 st.query_params.clear()
                 if auth_code:
                     flow = google_auth_oauthlib.flow.Flow.from_client_secrets_file(
                         self.secret_credentials_path, # replace with you json credentials from your google auth app
                         scopes=["openid", "https://www.googleapis.com/auth/userinfo.profile", "https://www.googleapis.com/auth/userinfo.email"],
```

### Comparing `streamlit-google-auth-1.1.6/src/streamlit_google_auth/cookie/__init__.py` & `streamlit-google-auth-1.1.7/src/streamlit_google_auth/cookie/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/PKG-INFO` & `streamlit-google-auth-1.1.7/src/streamlit_google_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.6
+Version: 1.1.7
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

