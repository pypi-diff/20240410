# Comparing `tmp/email-auth-remote-1.1.2.tar.gz` & `tmp/email-auth-remote-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-auth-remote-1.1.2.tar", last modified: Tue Apr  9 06:15:03 2024, max compression
+gzip compressed data, was "email-auth-remote-1.2.0.tar", last modified: Wed Apr 10 04:56:14 2024, max compression
```

## Comparing `email-auth-remote-1.1.2.tar` & `email-auth-remote-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-09 06:15:03.602213 email-auth-remote-1.1.2/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-09 06:15:03.602213 email-auth-remote-1.1.2/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2835 2024-04-09 06:14:20.000000 email-auth-remote-1.1.2/README.md
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-09 06:15:03.598213 email-auth-remote-1.1.2/email_auth_remote/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      351 2024-04-08 14:54:42.000000 email-auth-remote-1.1.2/email_auth_remote/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      142 2024-04-08 16:17:34.000000 email-auth-remote-1.1.2/email_auth_remote/admin.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1437 2024-04-08 14:51:55.000000 email-auth-remote-1.1.2/email_auth_remote/authentication.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2816 2024-04-08 14:53:29.000000 email-auth-remote-1.1.2/email_auth_remote/middleware.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1494 2024-04-08 14:45:35.000000 email-auth-remote-1.1.2/email_auth_remote/models.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      212 2024-04-08 07:54:28.000000 email-auth-remote-1.1.2/email_auth_remote/schema.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      727 2024-04-08 14:10:11.000000 email-auth-remote-1.1.2/email_auth_remote/settings.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-08 16:40:59.000000 email-auth-remote-1.1.2/email_auth_remote/urls.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1330 2024-04-08 14:48:28.000000 email-auth-remote-1.1.2/email_auth_remote/utils.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1318 2024-04-08 14:46:48.000000 email-auth-remote-1.1.2/email_auth_remote/views.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-09 06:15:03.598213 email-auth-remote-1.1.2/email_auth_remote.egg-info/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      519 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/SOURCES.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/dependency_links.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      110 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/requires.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/top_level.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      674 2024-04-09 06:07:16.000000 email-auth-remote-1.1.2/pyproject.toml
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-04-09 06:15:03.602213 email-auth-remote-1.1.2/setup.cfg
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 04:56:14.263478 email-auth-remote-1.2.0/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-10 04:56:14.263478 email-auth-remote-1.2.0/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     2835 2024-04-09 06:14:20.000000 email-auth-remote-1.2.0/README.md
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 04:56:14.259478 email-auth-remote-1.2.0/email_auth_remote/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      351 2024-04-08 14:54:42.000000 email-auth-remote-1.2.0/email_auth_remote/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      142 2024-04-08 16:17:34.000000 email-auth-remote-1.2.0/email_auth_remote/admin.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 04:56:14.263478 email-auth-remote-1.2.0/email_auth_remote/admin_override/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2024-04-09 17:58:40.000000 email-auth-remote-1.2.0/email_auth_remote/admin_override/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      177 2024-04-09 18:01:10.000000 email-auth-remote-1.2.0/email_auth_remote/admin_override/apps.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      311 2024-04-09 17:22:04.000000 email-auth-remote-1.2.0/email_auth_remote/apps.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1225 2024-04-10 03:56:04.000000 email-auth-remote-1.2.0/email_auth_remote/authentication.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-10 03:45:16.000000 email-auth-remote-1.2.0/email_auth_remote/context_processors.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      635 2024-04-10 04:18:27.000000 email-auth-remote-1.2.0/email_auth_remote/middleware.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1494 2024-04-08 14:45:35.000000 email-auth-remote-1.2.0/email_auth_remote/models.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      212 2024-04-08 07:54:28.000000 email-auth-remote-1.2.0/email_auth_remote/schema.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      424 2024-04-10 04:05:46.000000 email-auth-remote-1.2.0/email_auth_remote/settings.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-08 16:40:59.000000 email-auth-remote-1.2.0/email_auth_remote/urls.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      660 2024-04-10 03:55:41.000000 email-auth-remote-1.2.0/email_auth_remote/utils.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1159 2024-04-10 03:53:38.000000 email-auth-remote-1.2.0/email_auth_remote/views.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 04:56:14.263478 email-auth-remote-1.2.0/email_auth_remote.egg-info/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-10 04:56:14.000000 email-auth-remote-1.2.0/email_auth_remote.egg-info/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      671 2024-04-10 04:56:14.000000 email-auth-remote-1.2.0/email_auth_remote.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-04-10 04:56:14.000000 email-auth-remote-1.2.0/email_auth_remote.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      110 2024-04-10 04:56:14.000000 email-auth-remote-1.2.0/email_auth_remote.egg-info/requires.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-04-10 04:56:14.000000 email-auth-remote-1.2.0/email_auth_remote.egg-info/top_level.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      674 2024-04-10 04:55:49.000000 email-auth-remote-1.2.0/pyproject.toml
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-04-10 04:56:14.263478 email-auth-remote-1.2.0/setup.cfg
```

### Comparing `email-auth-remote-1.1.2/PKG-INFO` & `email-auth-remote-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.1.2
+Version: 1.2.0
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
```

### Comparing `email-auth-remote-1.1.2/README.md` & `email-auth-remote-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.2/email_auth_remote/models.py` & `email-auth-remote-1.2.0/email_auth_remote/models.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.2/email_auth_remote.egg-info/PKG-INFO` & `email-auth-remote-1.2.0/email_auth_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.1.2
+Version: 1.2.0
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
```

### Comparing `email-auth-remote-1.1.2/email_auth_remote.egg-info/SOURCES.txt` & `email-auth-remote-1.2.0/email_auth_remote.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 README.md
 pyproject.toml
 email_auth_remote/__init__.py
 email_auth_remote/admin.py
+email_auth_remote/apps.py
 email_auth_remote/authentication.py
+email_auth_remote/context_processors.py
 email_auth_remote/middleware.py
 email_auth_remote/models.py
 email_auth_remote/schema.py
 email_auth_remote/settings.py
 email_auth_remote/urls.py
 email_auth_remote/utils.py
 email_auth_remote/views.py
 email_auth_remote.egg-info/PKG-INFO
 email_auth_remote.egg-info/SOURCES.txt
 email_auth_remote.egg-info/dependency_links.txt
 email_auth_remote.egg-info/requires.txt
-email_auth_remote.egg-info/top_level.txt
+email_auth_remote.egg-info/top_level.txt
+email_auth_remote/admin_override/__init__.py
+email_auth_remote/admin_override/apps.py
```

### Comparing `email-auth-remote-1.1.2/pyproject.toml` & `email-auth-remote-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "email-auth-remote"
-version = "1.1.2"
+version = "1.2.0"
 description = "Django app for an endpoint authentication."
 readme = "README.md"
 requires-python = ">=3.11"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
```

