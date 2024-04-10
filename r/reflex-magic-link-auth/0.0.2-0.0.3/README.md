# Comparing `tmp/reflex-magic-link-auth-0.0.2.tar.gz` & `tmp/reflex-magic-link-auth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-magic-link-auth-0.0.2.tar", last modified: Thu Mar 21 18:59:48 2024, max compression
+gzip compressed data, was "reflex-magic-link-auth-0.0.3.tar", last modified: Wed Apr 10 19:13:39 2024, max compression
```

## Comparing `reflex-magic-link-auth-0.0.2.tar` & `reflex-magic-link-auth-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:59:48.363063 reflex-magic-link-auth-0.0.2/
--rw-r--r--   0 masen      (502) staff       (20)     3427 2024-03-21 18:59:48.362858 reflex-magic-link-auth-0.0.2/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)     2858 2024-03-15 06:20:37.000000 reflex-magic-link-auth-0.0.2/README.md
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:59:48.358502 reflex-magic-link-auth-0.0.2/custom_components/
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:59:48.360098 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/
--rw-r--r--   0 masen      (502) staff       (20)      382 2024-03-15 05:17:40.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/__init__.py
--rw-r--r--   0 masen      (502) staff       (20)      205 2024-03-15 04:47:59.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/constants.py
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:59:48.361720 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/models/
--rw-r--r--   0 masen      (502) staff       (20)      141 2024-03-15 05:00:10.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/models/__init__.py
--rw-r--r--   0 masen      (502) staff       (20)     2216 2024-03-15 06:40:04.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/models/record.py
--rw-r--r--   0 masen      (502) staff       (20)     1434 2024-03-15 06:56:23.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/models/session.py
--rw-r--r--   0 masen      (502) staff       (20)     1175 2024-03-15 06:54:39.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/page.py
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:59:48.362216 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/providers/
--rw-r--r--   0 masen      (502) staff       (20)       84 2024-03-15 05:59:56.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/providers/__init__.py
--rw-r--r--   0 masen      (502) staff       (20)     1542 2024-03-15 05:49:25.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/providers/mailgun.py
--rw-r--r--   0 masen      (502) staff       (20)     7200 2024-03-17 20:37:31.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/state.py
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-21 18:59:48.362532 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/
--rw-r--r--   0 masen      (502) staff       (20)     3427 2024-03-21 18:59:48.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)      851 2024-03-21 18:59:48.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/SOURCES.txt
--rw-r--r--   0 masen      (502) staff       (20)        1 2024-03-21 18:59:48.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/dependency_links.txt
--rw-r--r--   0 masen      (502) staff       (20)       46 2024-03-21 18:59:48.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/requires.txt
--rw-r--r--   0 masen      (502) staff       (20)       23 2024-03-21 18:59:48.000000 reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/top_level.txt
--rw-r--r--   0 masen      (502) staff       (20)      746 2024-03-21 18:58:01.000000 reflex-magic-link-auth-0.0.2/pyproject.toml
--rw-r--r--   0 masen      (502) staff       (20)       38 2024-03-21 18:59:48.363101 reflex-magic-link-auth-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:13:39.122019 reflex-magic-link-auth-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-10 19:13:39.122019 reflex-magic-link-auth-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:13:39.118019 reflex-magic-link-auth-0.0.3/custom_components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:13:39.118019 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:13:39.122019 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/models/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:13:39.122019 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/providers/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:13:39.122019 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-10 19:13:39.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-10 19:13:39.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:13:39.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 19:13:39.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 19:13:39.000000 reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-10 19:12:51.000000 reflex-magic-link-auth-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:13:39.122019 reflex-magic-link-auth-0.0.3/setup.cfg
```

### Comparing `reflex-magic-link-auth-0.0.2/PKG-INFO` & `reflex-magic-link-auth-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: reflex-magic-link-auth
-Version: 0.0.2
-Summary: Reflex custom component magic-link-auth
+Version: 0.0.3
+Summary: Login with magic links sent via email
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-magic-link-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `reflex-magic-link-auth-0.0.2/README.md` & `reflex-magic-link-auth-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/models/record.py` & `reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/models/record.py`

 * *Files identical despite different names*

### Comparing `reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/models/session.py` & `reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/models/session.py`

 * *Files identical despite different names*

### Comparing `reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/page.py` & `reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/page.py`

 * *Files identical despite different names*

### Comparing `reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/providers/mailgun.py` & `reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/providers/mailgun.py`

 * *Files identical despite different names*

### Comparing `reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth/state.py` & `reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth/state.py`

 * *Files identical despite different names*

### Comparing `reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/PKG-INFO` & `reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: reflex-magic-link-auth
-Version: 0.0.2
-Summary: Reflex custom component magic-link-auth
+Version: 0.0.3
+Summary: Login with magic links sent via email
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-magic-link-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `reflex-magic-link-auth-0.0.2/custom_components/reflex_magic_link_auth.egg-info/SOURCES.txt` & `reflex-magic-link-auth-0.0.3/custom_components/reflex_magic_link_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reflex-magic-link-auth-0.0.2/pyproject.toml` & `reflex-magic-link-auth-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,16 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-magic-link-auth"
-version = "0.0.2"
-description = "Reflex custom component magic-link-auth"
+version = "0.0.3"
+description = "Login with magic links sent via email"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
 keywords = [
     "reflex",
     "reflex-custom-components"]
```

