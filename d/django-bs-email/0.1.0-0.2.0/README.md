# Comparing `tmp/django-bs-email-0.1.0.tar.gz` & `tmp/django-bs-email-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bs-email-0.1.0.tar", last modified: Wed Apr 10 16:17:20 2024, max compression
+gzip compressed data, was "django-bs-email-0.2.0.tar", last modified: Wed Apr 10 17:18:49 2024, max compression
```

## Comparing `django-bs-email-0.1.0.tar` & `django-bs-email-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/django_bootstrap_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/django_bootstrap_email/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/django_bootstrap_email/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/templatetags/bootstrap_email.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/django_bootstrap_email/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/django_bs_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-10 16:17:20.000000 django-bs-email-0.1.0/django_bs_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-10 16:17:20.000000 django-bs-email-0.1.0/django_bs_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:17:20.000000 django-bs-email-0.1.0/django_bs_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 16:17:20.000000 django-bs-email-0.1.0/django_bs_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 16:17:20.000000 django-bs-email-0.1.0/django_bs_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:17:20.905656 django-bs-email-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 16:17:14.000000 django-bs-email-0.1.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:49.426465 django-bs-email-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-10 17:18:49.426465 django-bs-email-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:49.422465 django-bs-email-0.2.0/django_bootstrap_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/django_bootstrap_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/django_bootstrap_email/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:49.422465 django-bs-email-0.2.0/django_bootstrap_email/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/django_bootstrap_email/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/django_bootstrap_email/templatetags/bootstrap_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:49.426465 django-bs-email-0.2.0/django_bs_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-10 17:18:49.000000 django-bs-email-0.2.0/django_bs_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 17:18:49.000000 django-bs-email-0.2.0/django_bs_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:18:49.000000 django-bs-email-0.2.0/django_bs_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 17:18:49.000000 django-bs-email-0.2.0/django_bs_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 17:18:49.000000 django-bs-email-0.2.0/django_bs_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:18:49.426465 django-bs-email-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:49.422465 django-bs-email-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 17:18:39.000000 django-bs-email-0.2.0/tests/tests.py
```

### Comparing `django-bs-email-0.1.0/LICENSE` & `django-bs-email-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bs-email-0.1.0/django_bootstrap_email/templatetags/bootstrap_email.py` & `django-bs-email-0.2.0/django_bootstrap_email/templatetags/bootstrap_email.py`

 * *Files identical despite different names*

### Comparing `django-bs-email-0.1.0/pyproject.toml` & `django-bs-email-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-bs-email"
-version = "0.1.0"
+version = "0.2.0"
 description = "Django application with Bootstrap email template tag."
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [{name = "Jeremy Thompson"}]
 license = {file = "LICENSE"}
 dependencies = [
     "bootstrap-email",
```

### Comparing `django-bs-email-0.1.0/tests/tests.py` & `django-bs-email-0.2.0/tests/tests.py`

 * *Files identical despite different names*

