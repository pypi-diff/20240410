# Comparing `tmp/email-auth-remote-1.1.1.tar.gz` & `tmp/email-auth-remote-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-auth-remote-1.1.1.tar", last modified: Mon Apr  8 16:56:14 2024, max compression
+gzip compressed data, was "email-auth-remote-1.1.2.tar", last modified: Tue Apr  9 06:15:03 2024, max compression
```

## Comparing `email-auth-remote-1.1.1.tar` & `email-auth-remote-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-08 16:56:14.732490 email-auth-remote-1.1.1/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     3337 2024-04-08 16:56:14.732490 email-auth-remote-1.1.1/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2803 2024-04-08 16:53:21.000000 email-auth-remote-1.1.1/README.md
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-08 16:56:14.728490 email-auth-remote-1.1.1/email_auth_remote/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      351 2024-04-08 14:54:42.000000 email-auth-remote-1.1.1/email_auth_remote/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      142 2024-04-08 16:17:34.000000 email-auth-remote-1.1.1/email_auth_remote/admin.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1437 2024-04-08 14:51:55.000000 email-auth-remote-1.1.1/email_auth_remote/authentication.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2816 2024-04-08 14:53:29.000000 email-auth-remote-1.1.1/email_auth_remote/middleware.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1494 2024-04-08 14:45:35.000000 email-auth-remote-1.1.1/email_auth_remote/models.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      212 2024-04-08 07:54:28.000000 email-auth-remote-1.1.1/email_auth_remote/schema.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      727 2024-04-08 14:10:11.000000 email-auth-remote-1.1.1/email_auth_remote/settings.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-08 16:40:59.000000 email-auth-remote-1.1.1/email_auth_remote/urls.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1330 2024-04-08 14:48:28.000000 email-auth-remote-1.1.1/email_auth_remote/utils.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1318 2024-04-08 14:46:48.000000 email-auth-remote-1.1.1/email_auth_remote/views.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-08 16:56:14.732490 email-auth-remote-1.1.1/email_auth_remote.egg-info/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     3337 2024-04-08 16:56:14.000000 email-auth-remote-1.1.1/email_auth_remote.egg-info/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      519 2024-04-08 16:56:14.000000 email-auth-remote-1.1.1/email_auth_remote.egg-info/SOURCES.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-04-08 16:56:14.000000 email-auth-remote-1.1.1/email_auth_remote.egg-info/dependency_links.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       53 2024-04-08 16:56:14.000000 email-auth-remote-1.1.1/email_auth_remote.egg-info/requires.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-04-08 16:56:14.000000 email-auth-remote-1.1.1/email_auth_remote.egg-info/top_level.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      603 2024-04-08 16:54:09.000000 email-auth-remote-1.1.1/pyproject.toml
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-04-08 16:56:14.732490 email-auth-remote-1.1.1/setup.cfg
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-09 06:15:03.602213 email-auth-remote-1.1.2/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-09 06:15:03.602213 email-auth-remote-1.1.2/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     2835 2024-04-09 06:14:20.000000 email-auth-remote-1.1.2/README.md
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-09 06:15:03.598213 email-auth-remote-1.1.2/email_auth_remote/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      351 2024-04-08 14:54:42.000000 email-auth-remote-1.1.2/email_auth_remote/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      142 2024-04-08 16:17:34.000000 email-auth-remote-1.1.2/email_auth_remote/admin.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1437 2024-04-08 14:51:55.000000 email-auth-remote-1.1.2/email_auth_remote/authentication.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     2816 2024-04-08 14:53:29.000000 email-auth-remote-1.1.2/email_auth_remote/middleware.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1494 2024-04-08 14:45:35.000000 email-auth-remote-1.1.2/email_auth_remote/models.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      212 2024-04-08 07:54:28.000000 email-auth-remote-1.1.2/email_auth_remote/schema.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      727 2024-04-08 14:10:11.000000 email-auth-remote-1.1.2/email_auth_remote/settings.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-08 16:40:59.000000 email-auth-remote-1.1.2/email_auth_remote/urls.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1330 2024-04-08 14:48:28.000000 email-auth-remote-1.1.2/email_auth_remote/utils.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1318 2024-04-08 14:46:48.000000 email-auth-remote-1.1.2/email_auth_remote/views.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-09 06:15:03.598213 email-auth-remote-1.1.2/email_auth_remote.egg-info/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      519 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      110 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/requires.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-04-09 06:15:03.000000 email-auth-remote-1.1.2/email_auth_remote.egg-info/top_level.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      674 2024-04-09 06:07:16.000000 email-auth-remote-1.1.2/pyproject.toml
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-04-09 06:15:03.602213 email-auth-remote-1.1.2/setup.cfg
```

### Comparing `email-auth-remote-1.1.1/PKG-INFO` & `email-auth-remote-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.1.1
+Version: 1.1.2
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: Django>=4.2
 Requires-Dist: requests>=2.31
 Requires-Dist: djangorestframework>=3.14
+Requires-Dist: dj-rest-auth==5.1.0
+Requires-Dist: djangorestframework-simplejwt==5.3.1
 
 # Email Auth Remote
 
 Проект для интеграции МС авторизации с другими Django МС.
 
 ## Как пользоваться
 
 Добавить проект в INSTALLED_APPS.
 
 ```python
 # File: settings.py
 
 INSTALLED_APPS = [
     ...
+    "rest_framework_simplejwt",
     "email_auth_remote",
 ]
 ```
 
 В urlpatterns добавить include("email_auth_remote.urls") перед admin.site.urls.
 
 ```python
```

### Comparing `email-auth-remote-1.1.1/README.md` & `email-auth-remote-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Добавить проект в INSTALLED_APPS.
 
 ```python
 # File: settings.py
 
 INSTALLED_APPS = [
     ...
+    "rest_framework_simplejwt",
     "email_auth_remote",
 ]
 ```
 
 В urlpatterns добавить include("email_auth_remote.urls") перед admin.site.urls.
 
 ```python
```

### Comparing `email-auth-remote-1.1.1/email_auth_remote/authentication.py` & `email-auth-remote-1.1.2/email_auth_remote/authentication.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.1/email_auth_remote/middleware.py` & `email-auth-remote-1.1.2/email_auth_remote/middleware.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.1/email_auth_remote/models.py` & `email-auth-remote-1.1.2/email_auth_remote/models.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.1/email_auth_remote/settings.py` & `email-auth-remote-1.1.2/email_auth_remote/settings.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.1/email_auth_remote/utils.py` & `email-auth-remote-1.1.2/email_auth_remote/utils.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.1/email_auth_remote/views.py` & `email-auth-remote-1.1.2/email_auth_remote/views.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.1/email_auth_remote.egg-info/PKG-INFO` & `email-auth-remote-1.1.2/email_auth_remote.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.1.1
+Version: 1.1.2
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: Django>=4.2
 Requires-Dist: requests>=2.31
 Requires-Dist: djangorestframework>=3.14
+Requires-Dist: dj-rest-auth==5.1.0
+Requires-Dist: djangorestframework-simplejwt==5.3.1
 
 # Email Auth Remote
 
 Проект для интеграции МС авторизации с другими Django МС.
 
 ## Как пользоваться
 
 Добавить проект в INSTALLED_APPS.
 
 ```python
 # File: settings.py
 
 INSTALLED_APPS = [
     ...
+    "rest_framework_simplejwt",
     "email_auth_remote",
 ]
 ```
 
 В urlpatterns добавить include("email_auth_remote.urls") перед admin.site.urls.
 
 ```python
```

### Comparing `email-auth-remote-1.1.1/email_auth_remote.egg-info/SOURCES.txt` & `email-auth-remote-1.1.2/email_auth_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.1.1/pyproject.toml` & `email-auth-remote-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "email-auth-remote"
-version = "1.1.1"
+version = "1.1.2"
 description = "Django app for an endpoint authentication."
 readme = "README.md"
 requires-python = ">=3.11"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
@@ -12,14 +12,16 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
     "Django>=4.2",
     "requests>=2.31",
-    "djangorestframework>=3.14"
+    "djangorestframework>=3.14",
+    "dj-rest-auth==5.1.0",
+    "djangorestframework-simplejwt==5.3.1"
 ]
 
 
 [build-system]
 requires = ["setuptools>=69.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

