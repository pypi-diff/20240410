# Comparing `tmp/django-formsets-inside-form-0.1.0.tar.gz` & `tmp/django-formsets-inside-form-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formsets-inside-form-0.1.0.tar", last modified: Tue Apr  9 23:05:36 2024, max compression
+gzip compressed data, was "django-formsets-inside-form-0.1.1.tar", last modified: Wed Apr 10 00:02:36 2024, max compression
```

## Comparing `django-formsets-inside-form-0.1.0.tar` & `django-formsets-inside-form-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 deivid    (1000) deivid    (1000)        0 2024-04-09 23:05:36.066679 django-formsets-inside-form-0.1.0/
--rw-rw-r--   0 deivid    (1000) deivid    (1000)     1068 2024-04-09 21:21:49.000000 django-formsets-inside-form-0.1.0/LICENSE
--rw-r--r--   0 deivid    (1000) deivid    (1000)      320 2024-04-09 23:05:36.066679 django-formsets-inside-form-0.1.0/PKG-INFO
--rw-rw-r--   0 deivid    (1000) deivid    (1000)      777 2024-04-09 21:31:48.000000 django-formsets-inside-form-0.1.0/README.md
-drwxrwxr-x   0 deivid    (1000) deivid    (1000)        0 2024-04-09 23:05:36.066679 django-formsets-inside-form-0.1.0/django-formsets-inside-form/
--rw-rw-r--   0 deivid    (1000) deivid    (1000)       42 2024-04-09 21:30:48.000000 django-formsets-inside-form-0.1.0/django-formsets-inside-form/__init__.py
--rw-rw-r--   0 deivid    (1000) deivid    (1000)     1877 2024-04-09 21:30:27.000000 django-formsets-inside-form-0.1.0/django-formsets-inside-form/forms.py
-drwxrwxr-x   0 deivid    (1000) deivid    (1000)        0 2024-04-09 23:05:36.066679 django-formsets-inside-form-0.1.0/django_formsets_inside_form.egg-info/
--rw-r--r--   0 deivid    (1000) deivid    (1000)      320 2024-04-09 23:05:36.000000 django-formsets-inside-form-0.1.0/django_formsets_inside_form.egg-info/PKG-INFO
--rw-rw-r--   0 deivid    (1000) deivid    (1000)      357 2024-04-09 23:05:36.000000 django-formsets-inside-form-0.1.0/django_formsets_inside_form.egg-info/SOURCES.txt
--rw-rw-r--   0 deivid    (1000) deivid    (1000)        1 2024-04-09 23:05:36.000000 django-formsets-inside-form-0.1.0/django_formsets_inside_form.egg-info/dependency_links.txt
--rw-rw-r--   0 deivid    (1000) deivid    (1000)       12 2024-04-09 23:05:36.000000 django-formsets-inside-form-0.1.0/django_formsets_inside_form.egg-info/requires.txt
--rw-rw-r--   0 deivid    (1000) deivid    (1000)       28 2024-04-09 23:05:36.000000 django-formsets-inside-form-0.1.0/django_formsets_inside_form.egg-info/top_level.txt
--rw-rw-r--   0 deivid    (1000) deivid    (1000)       38 2024-04-09 23:05:36.066679 django-formsets-inside-form-0.1.0/setup.cfg
--rw-rw-r--   0 deivid    (1000) deivid    (1000)      426 2024-04-09 23:03:02.000000 django-formsets-inside-form-0.1.0/setup.py
+drwxrwxr-x   0 deivid    (1000) deivid    (1000)        0 2024-04-10 00:02:36.921850 django-formsets-inside-form-0.1.1/
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)     1068 2024-04-09 21:21:49.000000 django-formsets-inside-form-0.1.1/LICENSE
+-rw-r--r--   0 deivid    (1000) deivid    (1000)      320 2024-04-10 00:02:36.921850 django-formsets-inside-form-0.1.1/PKG-INFO
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)     2614 2024-04-09 23:58:35.000000 django-formsets-inside-form-0.1.1/README.rst
+drwxrwxr-x   0 deivid    (1000) deivid    (1000)        0 2024-04-10 00:02:36.921850 django-formsets-inside-form-0.1.1/django-formsets-inside-form/
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)       42 2024-04-09 21:30:48.000000 django-formsets-inside-form-0.1.1/django-formsets-inside-form/__init__.py
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)     1852 2024-04-10 00:01:43.000000 django-formsets-inside-form-0.1.1/django-formsets-inside-form/forms.py
+drwxrwxr-x   0 deivid    (1000) deivid    (1000)        0 2024-04-10 00:02:36.921850 django-formsets-inside-form-0.1.1/django_formsets_inside_form.egg-info/
+-rw-r--r--   0 deivid    (1000) deivid    (1000)      320 2024-04-10 00:02:36.000000 django-formsets-inside-form-0.1.1/django_formsets_inside_form.egg-info/PKG-INFO
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)      358 2024-04-10 00:02:36.000000 django-formsets-inside-form-0.1.1/django_formsets_inside_form.egg-info/SOURCES.txt
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)        1 2024-04-10 00:02:36.000000 django-formsets-inside-form-0.1.1/django_formsets_inside_form.egg-info/dependency_links.txt
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)       12 2024-04-10 00:02:36.000000 django-formsets-inside-form-0.1.1/django_formsets_inside_form.egg-info/requires.txt
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)       28 2024-04-10 00:02:36.000000 django-formsets-inside-form-0.1.1/django_formsets_inside_form.egg-info/top_level.txt
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)       38 2024-04-10 00:02:36.921850 django-formsets-inside-form-0.1.1/setup.cfg
+-rw-rw-r--   0 deivid    (1000) deivid    (1000)      426 2024-04-10 00:02:06.000000 django-formsets-inside-form-0.1.1/setup.py
```

### Comparing `django-formsets-inside-form-0.1.0/LICENSE` & `django-formsets-inside-form-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-formsets-inside-form-0.1.0/django-formsets-inside-form/forms.py` & `django-formsets-inside-form-0.1.1/django-formsets-inside-form/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from django import forms
 from django.db import transaction
 
 
 class FormsetsInsideFormMixin:
     """
     A mixin to be used with Django forms to manage inline formsets and atomic
     transactions in an integrated manner. This mixin provides functionality to handle
```

