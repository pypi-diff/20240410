# Comparing `tmp/reflex-google-auth-0.0.4.tar.gz` & `tmp/reflex-google-auth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-google-auth-0.0.4.tar", last modified: Mon Apr  1 19:16:19 2024, max compression
+gzip compressed data, was "reflex-google-auth-0.0.5.tar", last modified: Wed Apr 10 21:51:20 2024, max compression
```

## Comparing `reflex-google-auth-0.0.4.tar` & `reflex-google-auth-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.348198 reflex-google-auth-0.0.4/
--rw-r--r--   0 masenf     (501) staff       (20)      669 2024-04-01 19:16:19.347998 reflex-google-auth-0.0.4/PKG-INFO
--rw-r--r--   0 masenf     (501) staff       (20)      114 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/README.md
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.345464 reflex-google-auth-0.0.4/custom_components/
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.346831 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/
--rw-r--r--   0 masenf     (501) staff       (20)      291 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/__init__.py
--rw-r--r--   0 masenf     (501) staff       (20)      594 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/decorator.py
--rw-r--r--   0 masenf     (501) staff       (20)      794 2024-04-01 19:11:51.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/google_auth.py
--rw-r--r--   0 masenf     (501) staff       (20)     3800 2024-04-01 19:16:18.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/google_auth.pyi
--rw-r--r--   0 masenf     (501) staff       (20)     1486 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/state.py
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.347697 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/
--rw-r--r--   0 masenf     (501) staff       (20)      669 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 masenf     (501) staff       (20)      573 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 masenf     (501) staff       (20)        1 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 masenf     (501) staff       (20)       56 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/requires.txt
--rw-r--r--   0 masenf     (501) staff       (20)       19 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/top_level.txt
--rw-r--r--   0 masenf     (501) staff       (20)      740 2024-04-01 19:15:08.000000 reflex-google-auth-0.0.4/pyproject.toml
--rw-r--r--   0 masenf     (501) staff       (20)       38 2024-04-01 19:16:19.348236 reflex-google-auth-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:51:20.002693 reflex-google-auth-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-10 21:51:20.002693 reflex-google-auth-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-10 21:50:41.000000 reflex-google-auth-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:51:19.998693 reflex-google-auth-0.0.5/custom_components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:51:19.998693 reflex-google-auth-0.0.5/custom_components/reflex_google_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-10 21:50:41.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 21:50:41.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 21:50:41.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth/google_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-10 21:50:41.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:51:19.998693 reflex-google-auth-0.0.5/custom_components/reflex_google_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-10 21:51:19.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-10 21:51:19.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:51:19.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 21:51:19.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 21:51:19.000000 reflex-google-auth-0.0.5/custom_components/reflex_google_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 21:50:41.000000 reflex-google-auth-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:51:20.002693 reflex-google-auth-0.0.5/setup.cfg
```

### Comparing `reflex-google-auth-0.0.4/custom_components/reflex_google_auth/decorator.py` & `reflex-google-auth-0.0.5/custom_components/reflex_google_auth/decorator.py`

 * *Files identical despite different names*

### Comparing `reflex-google-auth-0.0.4/custom_components/reflex_google_auth/google_auth.py` & `reflex-google-auth-0.0.5/custom_components/reflex_google_auth/google_auth.py`

 * *Files identical despite different names*

### Comparing `reflex-google-auth-0.0.4/custom_components/reflex_google_auth/state.py` & `reflex-google-auth-0.0.5/custom_components/reflex_google_auth/state.py`

 * *Files identical despite different names*

### Comparing `reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/SOURCES.txt` & `reflex-google-auth-0.0.5/custom_components/reflex_google_auth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 README.md
 pyproject.toml
 custom_components/reflex_google_auth/__init__.py
 custom_components/reflex_google_auth/decorator.py
 custom_components/reflex_google_auth/google_auth.py
-custom_components/reflex_google_auth/google_auth.pyi
 custom_components/reflex_google_auth/state.py
 custom_components/reflex_google_auth.egg-info/PKG-INFO
 custom_components/reflex_google_auth.egg-info/SOURCES.txt
 custom_components/reflex_google_auth.egg-info/dependency_links.txt
 custom_components/reflex_google_auth.egg-info/requires.txt
 custom_components/reflex_google_auth.egg-info/top_level.txt
```

### Comparing `reflex-google-auth-0.0.4/pyproject.toml` & `reflex-google-auth-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,34 +3,32 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-google-auth"
-version = "0.0.4"
-description = "Reflex custom component google-auth"
+version = "0.0.5"
+description = "Sign in with Google"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
-keywords = [
-    "reflex",
-    "reflex-custom-components"]
+keywords = ["reflex", "reflex-custom-components"]
 
 dependencies = [
-    "reflex>=0.4.6a",
+    "reflex>=0.4.6",
     "google-auth[requests]",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
 ]
 
 [project.urls]
-Homepage = "https://github.com/martinxu9/reflex-google-auth"
+homepage = "https://github.com/masenf/reflex-google-auth"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.setuptools.packages.find]
 where = ["custom_components"]
```

