# Comparing `tmp/streamlit-google-auth-1.1.tar.gz` & `tmp/streamlit-google-auth-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-google-auth-1.1.tar", last modified: Wed Apr 10 07:09:40 2024, max compression
+gzip compressed data, was "streamlit-google-auth-1.1.1.tar", last modified: Wed Apr 10 07:44:28 2024, max compression
```

## Comparing `streamlit-google-auth-1.1.tar` & `streamlit-google-auth-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.508722 streamlit-google-auth-1.1/
--rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1/LICENSE
--rw-r--r--   0 adrien     (501) staff       (20)     5983 2024-04-10 07:09:40.508478 streamlit-google-auth-1.1/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1/README.md
--rw-r--r--   0 adrien     (501) staff       (20)      827 2024-04-10 07:09:27.000000 streamlit-google-auth-1.1/pyproject.toml
--rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 07:09:40.508767 streamlit-google-auth-1.1/setup.cfg
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.506293 streamlit-google-auth-1.1/src/
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.506895 streamlit-google-auth-1.1/src/streamlit_google_auth/
--rw-r--r--   0 adrien     (501) staff       (20)     5998 2024-04-09 15:56:05.000000 streamlit-google-auth-1.1/src/streamlit_google_auth/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.507948 streamlit-google-auth-1.1/src/streamlit_google_auth/cookie/
--rw-r--r--   0 adrien     (501) staff       (20)     3599 2024-04-09 15:36:22.000000 streamlit-google-auth-1.1/src/streamlit_google_auth/cookie/__init__.py
-drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.508229 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/
--rw-r--r--   0 adrien     (501) staff       (20)     5983 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/requires.txt
--rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/top_level.txt
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.331370 streamlit-google-auth-1.1.1/
+-rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1.1/LICENSE
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:44:28.331158 streamlit-google-auth-1.1.1/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1.1/README.md
+-rw-r--r--   0 adrien     (501) staff       (20)      829 2024-04-10 07:44:23.000000 streamlit-google-auth-1.1.1/pyproject.toml
+-rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 07:44:28.331415 streamlit-google-auth-1.1.1/setup.cfg
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.329432 streamlit-google-auth-1.1.1/src/
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.329963 streamlit-google-auth-1.1.1/src/streamlit_google_auth/
+-rw-r--r--   0 adrien     (501) staff       (20)     5998 2024-04-10 07:43:51.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.330730 streamlit-google-auth-1.1.1/src/streamlit_google_auth/cookie/
+-rw-r--r--   0 adrien     (501) staff       (20)     3654 2024-04-10 07:43:43.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth/cookie/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:44:28.330935 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/
+-rw-r--r--   0 adrien     (501) staff       (20)     5985 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/requires.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 07:44:28.000000 streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/top_level.txt
```

### Comparing `streamlit-google-auth-1.1/LICENSE` & `streamlit-google-auth-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1/PKG-INFO` & `streamlit-google-auth-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1
+Version: 1.1.1
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit-google-auth-1.1/README.md` & `streamlit-google-auth-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1/pyproject.toml` & `streamlit-google-auth-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit-google-auth"
-version = "1.1"
+version = "1.1.1"
 description = "Use Google authentification in streamlit"
 readme = "README.md"
 authors = [{ name = "Adrien Bouvais", email = "adrien.bouvais.pro@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `streamlit-google-auth-1.1/src/streamlit_google_auth/__init__.py` & `streamlit-google-auth-1.1.1/src/streamlit_google_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.1/src/streamlit_google_auth/cookie/__init__.py` & `streamlit-google-auth-1.1.1/src/streamlit_google_auth/cookie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             print(e)
 
     def set_cookie(self, name, email, picture, oauth_id):
         """
         Sets the re-authentication cookie.
         """
         self.exp_date = self._set_exp_date()
-        token = self._token_encode({'name': name, 'email': email, 'picture': picture, 'oauth_id': oauth_id})
+        token = self._token_encode(name, email, picture, oauth_id)
         self.cookie_manager.set(self.cookie_name, token,
                                 expires_at=datetime.now() + timedelta(days=self.cookie_expiry_days))
         
     def _set_exp_date(self) -> str:
         """
         Sets the re-authentication cookie's expiry date.
 
@@ -87,18 +87,18 @@
         except InvalidSignatureError as e:
             print(e)
             return False
         except DecodeError as e:
             print(e)
             return False
         
-    def _token_encode(self, email: str) -> str:
+    def _token_encode(self, name : str, email: str, picture: str, oauth_id: str) -> str:
         """
         Encodes the contents of the re-authentication cookie.
 
         Returns
         -------
         str
             Cookie used for password-less re-authentication.
         """
-        return jwt.encode({'email': email,
+        return jwt.encode({'email': email, 'name': name, 'picture': picture, 'oauth_id': oauth_id,
             'exp_date': self.exp_date}, self.cookie_key, algorithm='HS256')
```

### Comparing `streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/PKG-INFO` & `streamlit-google-auth-1.1.1/src/streamlit_google_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-google-auth
-Version: 1.1
+Version: 1.1.1
 Summary: Use Google authentification in streamlit
 Author-email: Adrien Bouvais <adrien.bouvais.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

