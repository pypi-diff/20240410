# Comparing `tmp/streamlit-google-auth-1.1.2.tar.gz` & `tmp/streamlit-google-auth-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-google-auth-1.1.2.tar", last modified: Wed Apr 10 07:52:38 2024, max compression
+gzip compressed data, was "streamlit-google-auth-1.1.3.tar", last modified: Wed Apr 10 08:07:36 2024, max compression
```

## Comparing `streamlit-google-auth-1.1.2.tar` & `streamlit-google-auth-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.787129 streamlit-google-auth-1.1.2/
--rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.2/LICENSE
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:52:38.786897 streamlit-google-auth-1.1.2/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.2/README.md
--rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 07:52:36.000000 streamlit-google-auth-1.1.2/pyproject.toml
--rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 07:52:38.787181 streamlit-google-auth-1.1.2/setup.cfg
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.784784 streamlit-google-auth-1.1.2/src/
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.785317 streamlit-google-auth-1.1.2/src/streamlit_google_auth/
--rw-r--r--   0 adrien     (501) staff       (20)     6038 2024-04-10 07:51:18.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.786342 streamlit-google-auth-1.1.2/src/streamlit_google_auth/cookie/
--rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth/cookie/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.786662 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/requires.txt
--rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/top_level.txt
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:07:36.878302 streamlit-google-auth-1.1.3/
+-rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.3/LICENSE
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:07:36.878035 streamlit-google-auth-1.1.3/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.3/README.md
+-rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 08:07:32.000000 streamlit-google-auth-1.1.3/pyproject.toml
+-rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 08:07:36.878347 streamlit-google-auth-1.1.3/setup.cfg
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:07:36.875877 streamlit-google-auth-1.1.3/src/
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:07:36.876381 streamlit-google-auth-1.1.3/src/streamlit_google_auth/
+-rw-r--r--   0 adrien     (501) staff       (20)     5102 2024-04-10 08:06:41.000000 streamlit-google-auth-1.1.3/src/streamlit_google_auth/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:07:36.877412 streamlit-google-auth-1.1.3/src/streamlit_google_auth/cookie/
+-rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.3/src/streamlit_google_auth/cookie/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:07:36.877795 streamlit-google-auth-1.1.3/src/streamlit_google_auth.egg-info/
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:07:36.000000 streamlit-google-auth-1.1.3/src/streamlit_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 08:07:36.000000 streamlit-google-auth-1.1.3/src/streamlit_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 08:07:36.000000 streamlit-google-auth-1.1.3/src/streamlit_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 08:07:36.000000 streamlit-google-auth-1.1.3/src/streamlit_google_auth.egg-info/requires.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 08:07:36.000000 streamlit-google-auth-1.1.3/src/streamlit_google_auth.egg-info/top_level.txt
```

### Comparing `streamlit-google-auth-1.1.2/LICENSE` & `streamlit-google-auth-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.2/PKG-INFO` & `streamlit-google-auth-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.2
+Version: 1.1.3
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit-google-auth-1.1.2/README.md` & `streamlit-google-auth-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.2/pyproject.toml` & `streamlit-google-auth-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit-google-auth"
-version = "1.1.2"
+version = "1.1.3"
 description = "Use Google authentification in streamlit"
 readme = "README.md"
 authors = [{ name = "Adrien Bouvais", email = "adrien.bouvais.pro@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `streamlit-google-auth-1.1.2/src/streamlit_google_auth/__init__.py` & `streamlit-google-auth-1.1.3/src/streamlit_google_auth/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,48 +30,35 @@
                 access_type="offline",
                 include_granted_scopes="true",
             )
         return authorization_url
 
     def login(self, color:Literal['white', 'blue']='blue', justify_content: str="center") -> tuple:
         if not st.session_state['connected']:
-            token = self.cookie_handler.get_cookie()
-            if token:
-                self.authentication_handler.execute_login(token=token)
-            time.sleep(0.7)
-            if not st.session_state['connected']:
-                flow = google_auth_oauthlib.flow.Flow.from_client_secrets_file(
-                    self.secret_credentials_path, # replace with you json credentials from your google auth app
-                    scopes=["openid", "https://www.googleapis.com/auth/userinfo.profile", "https://www.googleapis.com/auth/userinfo.email"],
-                    redirect_uri=self.redirect_uri,
-                )
-
-                authorization_url, state = flow.authorization_url(
-                        access_type="offline",
-                        include_granted_scopes="true",
-                    )
-                
+            flow = google_auth_oauthlib.flow.Flow.from_client_secrets_file(
+                self.secret_credentials_path, # replace with you json credentials from your google auth app
+                scopes=["openid", "https://www.googleapis.com/auth/userinfo.profile", "https://www.googleapis.com/auth/userinfo.email"],
+                redirect_uri=self.redirect_uri,
+            )
 
-                html_content = """<div style="display: flex; justify-content: p_justify_content;">
-<a href="p_authorization_url" target="_self" style="background-color: p_color_background; color: p_color_text; text-decoration: none; text-align: center; font-size: 16px; margin: 4px 2px; cursor: pointer; padding: 8px 12px; border-radius: 4px; display: flex; align-items: center;">
-    <img src="https://lh3.googleusercontent.com/COxitqgJr1sJnIDe8-jiKhxDx1FrYbtRHKJ9z_hELisAlapwE9LUPh6fcXIfb5vwpbMl4xl9H9TRFPc5NOO8Sb3VSgIBrfRYvW6cUA" alt="Google logo" style="margin-right: 8px; width: 26px; height: 26px; background-color: white; border: 2px solid white; border-radius: 4px;">
-    Sign in with Google
-</a>
-</div>"""
-                html_content = html_content.replace("p_justify_content", justify_content)
-                html_content = html_content.replace("p_authorization_url", authorization_url)
-                
-                if color == 'white':
-                    html_content = html_content.replace("p_color_background", "#ffffff")
-                    html_content = html_content.replace("p_color_text", "#000000")
-                else:
-                    html_content = html_content.replace("p_color_background", "#4285F4")
-                    html_content = html_content.replace("p_color_text", "#ffffff")
+            authorization_url, state = flow.authorization_url(
+                    access_type="offline",
+                    include_granted_scopes="true",
+                )
+            
+            html_content = f"""
+<div style="display: flex; justify-content: {justify_content};">
+    <a href="{authorization_url}" target="_self" style="background-color: {'#fff' if color == 'white' else '#4285f4'}; color: {'#000' if color == 'white' else '#fff'}; text-decoration: none; text-align: center; font-size: 16px; margin: 4px 2px; cursor: pointer; padding: 8px 12px; border-radius: 4px; display: flex; align-items: center;">
+        <img src="https://lh3.googleusercontent.com/COxitqgJr1sJnIDe8-jiKhxDx1FrYbtRHKJ9z_hELisAlapwE9LUPh6fcXIfb5vwpbMl4xl9H9TRFPc5NOO8Sb3VSgIBrfRYvW6cUA" alt="Google logo" style="margin-right: 8px; width: 26px; height: 26px; background-color: white; border: 2px solid white; border-radius: 4px;">
+        Sign in with Google
+    </a>
+</div>
+"""
 
-                st.markdown(html_content, unsafe_allow_html=True)
+            st.markdown(html_content, unsafe_allow_html=True)
 
     def check_authentification(self):
         if not st.session_state['connected']:
             token = self.cookie_handler.get_cookie()
             if token:
                 user_info = {
                     'name': token['name'],
@@ -79,38 +66,37 @@
                     'picture': token['picture'],
                     'id': token['oauth_id']
                 }
                 st.query_params.clear()
                 st.session_state["connected"] = True
                 st.session_state["user_info"] = user_info
                 st.session_state["oauth_id"] = user_info.get("id")
-            time.sleep(0.7)
+                return
             
-            if not st.session_state['connected']:
-                auth_code = st.query_params.get("code")
-                st.query_params.clear()
-                flow = google_auth_oauthlib.flow.Flow.from_client_secrets_file(
-                    self.secret_credentials_path, # replace with you json credentials from your google auth app
-                    scopes=["openid", "https://www.googleapis.com/auth/userinfo.profile", "https://www.googleapis.com/auth/userinfo.email"],
-                    redirect_uri=self.redirect_uri,
+            auth_code = st.query_params.get("code")
+            flow = google_auth_oauthlib.flow.Flow.from_client_secrets_file(
+                self.secret_credentials_path, # replace with you json credentials from your google auth app
+                scopes=["openid", "https://www.googleapis.com/auth/userinfo.profile", "https://www.googleapis.com/auth/userinfo.email"],
+                redirect_uri=self.redirect_uri,
+            )
+            if auth_code:
+                flow.fetch_token(code=auth_code)
+                credentials = flow.credentials
+                user_info_service = build(
+                    serviceName="oauth2",
+                    version="v2",
+                    credentials=credentials,
                 )
-                if auth_code:
-                    flow.fetch_token(code=auth_code)
-                    credentials = flow.credentials
-                    user_info_service = build(
-                        serviceName="oauth2",
-                        version="v2",
-                        credentials=credentials,
-                    )
-                    user_info = user_info_service.userinfo().get().execute()
+                user_info = user_info_service.userinfo().get().execute()
 
-                    self.cookie_handler.set_cookie(user_info.get("name"), user_info.get("email"), user_info.get("picture"), user_info.get("id"))
-                    st.session_state["connected"] = True
-                    st.session_state["oauth_id"] = user_info.get("id")
-                    st.session_state["user_info"] = user_info
+                self.cookie_handler.set_cookie(user_info.get("name"), user_info.get("email"), user_info.get("picture"), user_info.get("id"))
+                st.session_state["connected"] = True
+                st.session_state["oauth_id"] = user_info.get("id")
+                st.session_state["user_info"] = user_info
+                st.query_params.clear()
     
     def logout(self):
         st.session_state['logout'] = True
         st.session_state['name'] = None
         st.session_state['username'] = None
         st.session_state['connected'] = None
         self.cookie_handler.delete_cookie()
```

### Comparing `streamlit-google-auth-1.1.2/src/streamlit_google_auth/cookie/__init__.py` & `streamlit-google-auth-1.1.3/src/streamlit_google_auth/cookie/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/PKG-INFO` & `streamlit-google-auth-1.1.3/src/streamlit_google_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.2
+Version: 1.1.3
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

