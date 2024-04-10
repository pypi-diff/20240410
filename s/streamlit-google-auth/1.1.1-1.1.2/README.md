# Comparing `tmp/streamlit-google-auth-1.1.1.tar.gz` & `tmp/streamlit-google-auth-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-google-auth-1.1.1.tar", last modified: Wed Apr 10 07:44:28 2024, max compression
+gzip compressed data, was "streamlit-google-auth-1.1.2.tar", last modified: Wed Apr 10 07:52:38 2024, max compression
```

## Comparing `streamlit-google-auth-1.1.1.tar` & `streamlit-google-auth-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.331370 streamlit-google-auth-1.1.1/
--rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.1/LICENSE
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:44:28.331158 streamlit-google-auth-1.1.1/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.1/README.md
--rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 07:44:23.000000 streamlit-google-auth-1.1.1/pyproject.toml
--rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 07:44:28.331415 streamlit-google-auth-1.1.1/setup.cfg
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.329432 streamlit-google-auth-1.1.1/src/
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.329963 streamlit-google-auth-1.1.1/src/streamlit_google_auth/
--rw-r--r--   0 adrien     (501) staff       (20)     5998 2024-04-10 07:43:51.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.330730 streamlit-google-auth-1.1.1/src/streamlit_google_auth/cookie/
--rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth/cookie/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.330935 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/
--rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/requires.txt
--rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/top_level.txt
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.787129 streamlit-google-auth-1.1.2/
+-rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.2/LICENSE
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:52:38.786897 streamlit-google-auth-1.1.2/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.2/README.md
+-rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 07:52:36.000000 streamlit-google-auth-1.1.2/pyproject.toml
+-rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 07:52:38.787181 streamlit-google-auth-1.1.2/setup.cfg
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.784784 streamlit-google-auth-1.1.2/src/
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.785317 streamlit-google-auth-1.1.2/src/streamlit_google_auth/
+-rw-r--r--   0 adrien     (501) staff       (20)     6038 2024-04-10 07:51:18.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.786342 streamlit-google-auth-1.1.2/src/streamlit_google_auth/cookie/
+-rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth/cookie/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:52:38.786662 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/requires.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 07:52:38.000000 streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/top_level.txt
```

### Comparing `streamlit-google-auth-1.1.1/LICENSE` & `streamlit-google-auth-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.1/PKG-INFO` & `streamlit-google-auth-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.1
+Version: 1.1.2
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit-google-auth-1.1.1/README.md` & `streamlit-google-auth-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.1/pyproject.toml` & `streamlit-google-auth-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit-google-auth"
-version = "1.1.1"
+version = "1.1.2"
 description = "Use Google authentification in streamlit"
 readme = "README.md"
 authors = [{ name = "Adrien Bouvais", email = "adrien.bouvais.pro@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `streamlit-google-auth-1.1.1/src/streamlit_google_auth/__init__.py` & `streamlit-google-auth-1.1.2/src/streamlit_google_auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             if token:
                 user_info = {
                     'name': token['name'],
                     'email': token['email'],
                     'picture': token['picture'],
                     'id': token['oauth_id']
                 }
+                st.query_params.clear()
                 st.session_state["connected"] = True
                 st.session_state["user_info"] = user_info
                 st.session_state["oauth_id"] = user_info.get("id")
             time.sleep(0.7)
             
             if not st.session_state['connected']:
                 auth_code = st.query_params.get("code")
```

### Comparing `streamlit-google-auth-1.1.1/src/streamlit_google_auth/cookie/__init__.py` & `streamlit-google-auth-1.1.2/src/streamlit_google_auth/cookie/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/PKG-INFO` & `streamlit-google-auth-1.1.2/src/streamlit_google_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1.1
+Version: 1.1.2
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

