# Comparing `tmp/streamlit-google-auth-1.1.5.tar.gz` & `tmp/streamlit-google-auth-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-google-auth-1.1.5.tar", last modified: Wed Apr 10 08:20:00 2024, max compression
+gzip compressed data, was "streamlit-google-auth-1.1.6.tar", last modified: Wed Apr 10 08:27:47 2024, max compression
```

## Comparing `streamlit-google-auth-1.1.5.tar` & `streamlit-google-auth-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:20:00.130766 streamlit-google-auth-1.1.5/
--rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.5/LICENSE
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:20:00.130525 streamlit-google-auth-1.1.5/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.5/README.md
--rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 08:19:51.000000 streamlit-google-auth-1.1.5/pyproject.toml
--rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 08:20:00.130809 streamlit-google-auth-1.1.5/setup.cfg
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:20:00.128471 streamlit-google-auth-1.1.5/src/
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:20:00.129109 streamlit-google-auth-1.1.5/src/streamlit_google_auth/
--rw-r--r--   0 adrien     (501) staff       (20)     5289 2024-04-10 08:19:38.000000 streamlit-google-auth-1.1.5/src/streamlit_google_auth/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:20:00.129889 streamlit-google-auth-1.1.5/src/streamlit_google_auth/cookie/
--rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.5/src/streamlit_google_auth/cookie/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:20:00.130281 streamlit-google-auth-1.1.5/src/streamlit_google_auth.egg-info/
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:20:00.000000 streamlit-google-auth-1.1.5/src/streamlit_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 08:20:00.000000 streamlit-google-auth-1.1.5/src/streamlit_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 08:20:00.000000 streamlit-google-auth-1.1.5/src/streamlit_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 08:20:00.000000 streamlit-google-auth-1.1.5/src/streamlit_google_auth.egg-info/requires.txt
--rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 08:20:00.000000 streamlit-google-auth-1.1.5/src/streamlit_google_auth.egg-info/top_level.txt
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.200280 streamlit-google-auth-1.1.6/
+-rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.6/LICENSE
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:27:47.200055 streamlit-google-auth-1.1.6/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.6/README.md
+-rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 08:27:43.000000 streamlit-google-auth-1.1.6/pyproject.toml
+-rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 08:27:47.200323 streamlit-google-auth-1.1.6/setup.cfg
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.198235 streamlit-google-auth-1.1.6/src/
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.198754 streamlit-google-auth-1.1.6/src/streamlit_google_auth/
+-rw-r--r--   0 adrien     (501) staff       (20)     5320 2024-04-10 08:27:28.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.199477 streamlit-google-auth-1.1.6/src/streamlit_google_auth/cookie/
+-rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth/cookie/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 08:27:47.199825 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/requires.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 08:27:47.000000 streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/top_level.txt
```

### Comparing `streamlit-google-auth-1.1.5/LICENSE` & `streamlit-google-auth-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.5/PKG-INFO` & `streamlit-google-auth-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.5
+Version: 1.1.6
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit-google-auth-1.1.5/README.md` & `streamlit-google-auth-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.5/pyproject.toml` & `streamlit-google-auth-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit-google-auth"
-version = "1.1.5"
+version = "1.1.6"
 description = "Use Google authentification in streamlit"
 readme = "README.md"
 authors = [{ name = "Adrien Bouvais", email = "adrien.bouvais.pro@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `streamlit-google-auth-1.1.5/src/streamlit_google_auth/__init__.py` & `streamlit-google-auth-1.1.6/src/streamlit_google_auth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,19 @@
                     user_info_service = build(
                         serviceName="oauth2",
                         version="v2",
                         credentials=credentials,
                     )
                     user_info = user_info_service.userinfo().get().execute()
 
-                    self.cookie_handler.set_cookie(user_info.get("name"), user_info.get("email"), user_info.get("picture"), user_info.get("id"))
                     st.session_state["connected"] = True
                     st.session_state["oauth_id"] = user_info.get("id")
                     st.session_state["user_info"] = user_info
+                    self.cookie_handler.set_cookie(user_info.get("name"), user_info.get("email"), user_info.get("picture"), user_info.get("id"))
+                    st.rerun()
     
     def logout(self):
         st.session_state['logout'] = True
         st.session_state['name'] = None
         st.session_state['username'] = None
         st.session_state['connected'] = None
         self.cookie_handler.delete_cookie()
```

### Comparing `streamlit-google-auth-1.1.5/src/streamlit_google_auth/cookie/__init__.py` & `streamlit-google-auth-1.1.6/src/streamlit_google_auth/cookie/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.5/src/streamlit_google_auth.egg-info/PKG-INFO` & `streamlit-google-auth-1.1.6/src/streamlit_google_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.5
+Version: 1.1.6
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

