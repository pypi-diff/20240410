# Comparing `tmp/wagtail-liveedit-0.0.8.tar.gz` & `tmp/wagtail-liveedit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-liveedit-0.0.8.tar", last modified: Wed Sep 27 22:52:01 2023, max compression
+gzip compressed data, was "wagtail-liveedit-0.0.9.tar", last modified: Fri Feb 16 13:45:48 2024, max compression
```

## Comparing `wagtail-liveedit-0.0.8.tar` & `wagtail-liveedit-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      180 2023-01-25 17:52:22.000000 wagtail-liveedit-0.0.8/DEVELOPMENT.md
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     1067 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.8/LICENSE
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      151 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.8/MANIFEST.in
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      422 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/PKG-INFO
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     2882 2023-09-27 22:43:01.000000 wagtail-liveedit-0.0.8/README.md
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/liveedit/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.8/liveedit/__init__.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.8/liveedit/models.py
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.546005 wagtail-liveedit-0.0.8/liveedit/static/
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/liveedit/static/css/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     2235 2023-09-27 22:31:43.000000 wagtail-liveedit-0.0.8/liveedit/static/css/liveedit.css
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/liveedit/static/js/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     8833 2023-09-27 10:29:30.000000 wagtail-liveedit-0.0.8/liveedit/static/js/liveedit.js
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.546005 wagtail-liveedit-0.0.8/liveedit/templates/
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/liveedit/templates/liveedit/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     1888 2023-02-16 10:18:23.000000 wagtail-liveedit-0.0.8/liveedit/templates/liveedit/edit_panel.html
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/liveedit/templatetags/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.8/liveedit/templatetags/__init__.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     5288 2023-06-26 16:28:37.000000 wagtail-liveedit-0.0.8/liveedit/templatetags/liveedit.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      227 2022-04-11 09:36:59.000000 wagtail-liveedit-0.0.8/liveedit/urls.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      656 2022-06-13 08:40:43.000000 wagtail-liveedit-0.0.8/liveedit/utils.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)    10324 2023-09-27 22:30:58.000000 wagtail-liveedit-0.0.8/liveedit/views.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)       38 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/setup.cfg
--rwxrwxr-x   0 jonny     (1000) jonny     (1000)      667 2023-09-27 22:51:39.000000 wagtail-liveedit-0.0.8/setup.py
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/tests/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 20:29:38.000000 wagtail-liveedit-0.0.8/tests/__init__.py
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/tests/migrations/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     1358 2023-06-14 12:48:46.000000 wagtail-liveedit-0.0.8/tests/migrations/0001_initial.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-11 12:23:42.000000 wagtail-liveedit-0.0.8/tests/migrations/__init__.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     1673 2023-09-27 22:15:33.000000 wagtail-liveedit-0.0.8/tests/models.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     1767 2023-09-27 19:47:16.000000 wagtail-liveedit-0.0.8/tests/settings.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     9604 2023-09-27 22:22:28.000000 wagtail-liveedit-0.0.8/tests/test_backend.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)     5511 2023-09-27 19:46:00.000000 wagtail-liveedit-0.0.8/tests/test_frontend.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      501 2023-06-14 12:50:01.000000 wagtail-liveedit-0.0.8/tests/urls.py
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      253 2022-01-03 11:25:06.000000 wagtail-liveedit-0.0.8/tests/views.py
-drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2023-09-27 22:52:01.548005 wagtail-liveedit-0.0.8/wagtail_liveedit.egg-info/
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      422 2023-09-27 22:52:01.000000 wagtail-liveedit-0.0.8/wagtail_liveedit.egg-info/PKG-INFO
--rw-rw-r--   0 jonny     (1000) jonny     (1000)      709 2023-09-27 22:52:01.000000 wagtail-liveedit-0.0.8/wagtail_liveedit.egg-info/SOURCES.txt
--rw-rw-r--   0 jonny     (1000) jonny     (1000)        1 2023-09-27 22:52:01.000000 wagtail-liveedit-0.0.8/wagtail_liveedit.egg-info/dependency_links.txt
--rw-rw-r--   0 jonny     (1000) jonny     (1000)       22 2023-09-27 22:52:01.000000 wagtail-liveedit-0.0.8/wagtail_liveedit.egg-info/requires.txt
--rw-rw-r--   0 jonny     (1000) jonny     (1000)        9 2023-09-27 22:52:01.000000 wagtail-liveedit-0.0.8/wagtail_liveedit.egg-info/top_level.txt
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.402065 wagtail-liveedit-0.0.9/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      319 2024-02-16 13:45:10.000000 wagtail-liveedit-0.0.9/DEVELOPMENT.md
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     1067 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.9/LICENSE
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      151 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.9/MANIFEST.in
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      422 2024-02-16 13:45:48.402065 wagtail-liveedit-0.0.9/PKG-INFO
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     2860 2024-02-16 13:41:28.000000 wagtail-liveedit-0.0.9/README.md
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/liveedit/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.9/liveedit/__init__.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.9/liveedit/models.py
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/liveedit/static/
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/liveedit/static/css/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     2235 2023-09-27 22:31:43.000000 wagtail-liveedit-0.0.9/liveedit/static/css/liveedit.css
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/liveedit/static/js/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     8833 2023-09-27 10:29:30.000000 wagtail-liveedit-0.0.9/liveedit/static/js/liveedit.js
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/liveedit/templates/
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/liveedit/templates/liveedit/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     1888 2023-02-16 10:18:23.000000 wagtail-liveedit-0.0.9/liveedit/templates/liveedit/edit_panel.html
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/liveedit/templatetags/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 09:52:56.000000 wagtail-liveedit-0.0.9/liveedit/templatetags/__init__.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     5288 2023-06-26 16:28:37.000000 wagtail-liveedit-0.0.9/liveedit/templatetags/liveedit.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      227 2022-04-11 09:36:59.000000 wagtail-liveedit-0.0.9/liveedit/urls.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      656 2022-06-13 08:40:43.000000 wagtail-liveedit-0.0.9/liveedit/utils.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)    10257 2024-02-16 13:24:25.000000 wagtail-liveedit-0.0.9/liveedit/views.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)       38 2024-02-16 13:45:48.402065 wagtail-liveedit-0.0.9/setup.cfg
+-rwxrwxr-x   0 jonny     (1000) jonny     (1000)      667 2024-02-16 13:43:36.000000 wagtail-liveedit-0.0.9/setup.py
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.398065 wagtail-liveedit-0.0.9/tests/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-10 20:29:38.000000 wagtail-liveedit-0.0.9/tests/__init__.py
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.402065 wagtail-liveedit-0.0.9/tests/migrations/
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     1358 2023-06-14 12:48:46.000000 wagtail-liveedit-0.0.9/tests/migrations/0001_initial.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)        0 2021-12-11 12:23:42.000000 wagtail-liveedit-0.0.9/tests/migrations/__init__.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     1796 2024-02-16 13:39:24.000000 wagtail-liveedit-0.0.9/tests/models.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     1826 2024-02-16 13:33:58.000000 wagtail-liveedit-0.0.9/tests/settings.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     9604 2023-09-27 22:22:28.000000 wagtail-liveedit-0.0.9/tests/test_backend.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)     5511 2023-09-27 19:46:00.000000 wagtail-liveedit-0.0.9/tests/test_frontend.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      544 2024-02-16 13:35:33.000000 wagtail-liveedit-0.0.9/tests/urls.py
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      253 2022-01-03 11:25:06.000000 wagtail-liveedit-0.0.9/tests/views.py
+drwxrwxr-x   0 jonny     (1000) jonny     (1000)        0 2024-02-16 13:45:48.402065 wagtail-liveedit-0.0.9/wagtail_liveedit.egg-info/
+-rw-r--r--   0 jonny     (1000) jonny     (1000)      422 2024-02-16 13:45:48.000000 wagtail-liveedit-0.0.9/wagtail_liveedit.egg-info/PKG-INFO
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)      709 2024-02-16 13:45:48.000000 wagtail-liveedit-0.0.9/wagtail_liveedit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)        1 2024-02-16 13:45:48.000000 wagtail-liveedit-0.0.9/wagtail_liveedit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)       22 2024-02-16 13:45:48.000000 wagtail-liveedit-0.0.9/wagtail_liveedit.egg-info/requires.txt
+-rw-rw-r--   0 jonny     (1000) jonny     (1000)        9 2024-02-16 13:45:48.000000 wagtail-liveedit-0.0.9/wagtail_liveedit.egg-info/top_level.txt
```

### Comparing `wagtail-liveedit-0.0.8/LICENSE` & `wagtail-liveedit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/README.md` & `wagtail-liveedit-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 Wagtail (see compatibility matrix below)
 Python 3.8+
 
 ## Compatibility matrix
 
 Wagtail version | Passing tests?
 ----------------|---------------
-4.1.7           | :heavy_check_mark:
-5.1.2           | :heavy_check_mark:
-5.0.3           | :heavy_check_mark:
+6.0.1           | :heavy_check_mark:
+5.2.3           | :heavy_check_mark:
+5.1.3           | :heavy_check_mark:
+5.0.5           | :heavy_check_mark:
+4.1.9           | :heavy_check_mark:
 4.2.4           | :heavy_check_mark:
 4.0.4           | :heavy_check_mark:
-2.16.3          | :heavy_check_mark:
-2.15.6          | :x:
-3.0.3           | :heavy_check_mark:
 
 ## Installation
 
 1. Add `'liveedit'` to INSTALLED_APPS.
 
 2. Add:
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 # wagtail-liveedit Allow StreamField blocks to be edited via your Wagtail
 site's frontend. ## Demo ## Requirements Wagtail (see compatibility matrix
 below) Python 3.8+ ## Compatibility matrix Wagtail version | Passing tests? ---
--------------|--------------- 4.1.7 | :heavy_check_mark: 5.1.2 | :
-heavy_check_mark: 5.0.3 | :heavy_check_mark: 4.2.4 | :heavy_check_mark: 4.0.4 |
-:heavy_check_mark: 2.16.3 | :heavy_check_mark: 2.15.6 | :x: 3.0.3 | :
-heavy_check_mark: ## Installation 1. Add `'liveedit'` to INSTALLED_APPS. 2.
-Add: ``` url(r'^__liveedit__/', include('liveedit.urls')), ``` to your app's
-`urls.py` urlpatterns list 3. In your templates, when rendering StreamFields,
-replace: `{% include_block block %}` with `{% liveedit_include_block block
-object=page field="body" %}` where `page` is the model instance to which the
-StreamField belongs, and `"body"` is the name of the StreamField on that model
-instance. (Also add `liveedit` to the `{% load ... %}` at the top). 4. In your
-block templates, add `{% liveedit_attributes %}` inside the outermost opening
-HTML tag. For example: ```
+-------------|--------------- 6.0.1 | :heavy_check_mark: 5.2.3 | :
+heavy_check_mark: 5.1.3 | :heavy_check_mark: 5.0.5 | :heavy_check_mark: 4.1.9 |
+:heavy_check_mark: 4.2.4 | :heavy_check_mark: 4.0.4 | :heavy_check_mark: ##
+Installation 1. Add `'liveedit'` to INSTALLED_APPS. 2. Add: ``` url
+(r'^__liveedit__/', include('liveedit.urls')), ``` to your app's `urls.py`
+urlpatterns list 3. In your templates, when rendering StreamFields, replace: `
+{% include_block block %}` with `{% liveedit_include_block block object=page
+field="body" %}` where `page` is the model instance to which the StreamField
+belongs, and `"body"` is the name of the StreamField on that model instance.
+(Also add `liveedit` to the `{% load ... %}` at the top). 4. In your block
+templates, add `{% liveedit_attributes %}` inside the outermost opening HTML
+tag. For example: ```
 % liveedit_attributes %}> ...
 ``` (Also add `liveedit` to the `{% load ... %}` at the top). 5. In your base
 template add: `{% liveedit_css %}` with the style tags in the `
 ` and, `{% liveedit_js %}` just before the closing `
 ` tag. (Also add `liveedit` to the `{% load ... %}` at the top). ## How it
 works When each block is rendered in your templates, it is annotated with a
 reference to the underlying StreamValue which contains the block data. This
```

### Comparing `wagtail-liveedit-0.0.8/liveedit/static/css/liveedit.css` & `wagtail-liveedit-0.0.9/liveedit/static/css/liveedit.css`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/liveedit/static/js/liveedit.js` & `wagtail-liveedit-0.0.9/liveedit/static/js/liveedit.js`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/liveedit/templates/liveedit/edit_panel.html` & `wagtail-liveedit-0.0.9/liveedit/templates/liveedit/edit_panel.html`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/liveedit/templatetags/liveedit.py` & `wagtail-liveedit-0.0.9/liveedit/templatetags/liveedit.py`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/liveedit/utils.py` & `wagtail-liveedit-0.0.9/liveedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/liveedit/views.py` & `wagtail-liveedit-0.0.9/liveedit/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import render
 from django.template.exceptions import TemplateDoesNotExist
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
 from django.views.decorators.csrf import csrf_exempt
 
-from wagtail.contrib.modeladmin.helpers import PermissionHelper
-
 import wagtail
 if wagtail.VERSION < (3,):
     from wagtail.core.blocks import BlockWidget
     from wagtail.core.models import Page
     from wagtail.core.blocks.stream_block import StreamValue
 else:
     from wagtail.blocks import BlockWidget
@@ -112,15 +110,15 @@
                 rev.save()
     return obj, save
 
 def check_can_edit(user, obj):
     if hasattr(obj, 'permissions_for_user'):
         if not obj.permissions_for_user(user).can_edit():
             raise PermissionDenied
-    elif not PermissionHelper(obj).user_can_edit_obj(user, obj):
+    elif not user.has_perm("%s.change" % obj._meta.app_label):
         raise PermissionDenied
 
 def render_edit_panel(request, d):
     # Steal all of the <script> and stylesheet tags from the admin base template
     admin_base = render_to_string("wagtailadmin/admin_base.html", request=request)
     script_tags = mark_safe("\n".join(re.findall('<script[^>]*>.*?</script>', admin_base, re.DOTALL)))
     stylesheet_tags = mark_safe("\n".join(re.findall('<link rel="stylesheet"[^>]+/?>', admin_base, re.DOTALL)))
```

### Comparing `wagtail-liveedit-0.0.8/setup.py` & `wagtail-liveedit-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='wagtail-liveedit',
-      version='0.0.8',
+      version='0.0.9',
       description='Live editing add-on for Wagtail CMS',
       author='jonny5532',
       license='MIT',
       url='https://github.com/jonny5532/wagtail-liveedit',
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Framework :: Wagtail",
       ],
       packages=find_packages(exclude=['tests', 'tests.migrations']),
       include_package_data=True,
       install_requires=[
-          'wagtail>=2.16,<=5.1.2',
+          'wagtail>=2.16,<=6.0.1',
       ],
      )
```

### Comparing `wagtail-liveedit-0.0.8/tests/migrations/0001_initial.py` & `wagtail-liveedit-0.0.9/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/tests/models.py` & `wagtail-liveedit-0.0.9/tests/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import wagtail
+from wagtail.admin.panels import FieldPanel
 try:
     from wagtail import blocks
     from wagtail.fields import StreamField
     from wagtail.models import Page
 except ImportError:
     # Wagtail <5
     from wagtail.core import blocks
@@ -48,7 +49,10 @@
 
         ('required', blocks.StructBlock([
             ('text', blocks.TextBlock(required=True)),
         ])),
 
     ], **STREAMFIELD_ARGS, null=True, blank=True)
 
+    content_panels = Page.content_panels + [
+        FieldPanel("body"),
+    ]
```

### Comparing `wagtail-liveedit-0.0.8/tests/settings.py` & `wagtail-liveedit-0.0.9/tests/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     'django.contrib.staticfiles',
 
 ]
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': ':memory:',
+        'NAME': os.getenv('DATABASE_FILE', ':memory:'),
     }
 }
 
 SECRET_KEY = 'secretkey'
 
 MIDDLEWARE = [
 	'django.middleware.security.SecurityMiddleware',
@@ -72,8 +72,10 @@
 
 ROOT_URLCONF = 'tests.urls'
 
 STATIC_URL = '/static/'
 
 STATIC_ROOT = os.path.join(BASE_DIR, 'static')
 
+WAGTAIL_SITE_NAME = "Example"
+
 WAGTAILADMIN_BASE_URL = "https://example.com/"
```

### Comparing `wagtail-liveedit-0.0.8/tests/test_backend.py` & `wagtail-liveedit-0.0.9/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/tests/test_frontend.py` & `wagtail-liveedit-0.0.9/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `wagtail-liveedit-0.0.8/wagtail_liveedit.egg-info/SOURCES.txt` & `wagtail-liveedit-0.0.9/wagtail_liveedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

