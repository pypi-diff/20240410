# Comparing `tmp/djrender-0.1a11.tar.gz` & `tmp/djrender-0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djrender-0.1a11.tar", last modified: Thu Mar 21 14:27:14 2024, max compression
+gzip compressed data, was "djrender-0.1b1.tar", last modified: Tue Apr  9 12:36:55 2024, max compression
```

## Comparing `djrender-0.1a11.tar` & `djrender-0.1b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.654393 djrender-0.1a11/
--rw-rw-r--   0 karl      (1000) karl      (1000)      103 2024-03-21 13:29:03.000000 djrender-0.1a11/MANIFEST.in
--rw-rw-r--   0 karl      (1000) karl      (1000)     1145 2024-03-21 14:27:14.654393 djrender-0.1a11/PKG-INFO
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.646393 djrender-0.1a11/djangorender/
--rw-rw-r--   0 karl      (1000) karl      (1000)      470 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      343 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3251 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/decorators.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3147 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/response.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.642393 djrender-0.1a11/djangorender/static/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.642393 djrender-0.1a11/djangorender/static/djangorender/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.646393 djrender-0.1a11/djangorender/static/djangorender/fonts/
--rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/static/djangorender/fonts/.gitignore
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.650393 djrender-0.1a11/djangorender/static/djangorender/images/
--rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/static/djangorender/images/.gitignore
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.650393 djrender-0.1a11/djangorender/static/djangorender/js/
--rw-rw-r--   0 karl      (1000) karl      (1000)       17 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/static/djangorender/js/.gitignore
--rw-rw-r--   0 karl      (1000) karl      (1000)     1754 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/telepath.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.646393 djrender-0.1a11/djangorender/templates/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.650393 djrender-0.1a11/djangorender/templates/djangorender/
--rw-rw-r--   0 karl      (1000) karl      (1000)     3497 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/templates/djangorender/bootstrap.html
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.650393 djrender-0.1a11/djangorender/test/
--rw-rw-r--   0 karl      (1000) karl      (1000)       72 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/test/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      183 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/test/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3650 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/test/settings.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.650393 djrender-0.1a11/djangorender/test/tests/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/test/tests/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/test/urls.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.650393 djrender-0.1a11/djangorender/ui/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/ui/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3594 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/ui/forms.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1438 2024-03-21 13:29:03.000000 djrender-0.1a11/djangorender/views.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-03-21 14:27:14.650393 djrender-0.1a11/djrender.egg-info/
--rw-rw-r--   0 karl      (1000) karl      (1000)     1145 2024-03-21 14:27:14.000000 djrender-0.1a11/djrender.egg-info/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)      755 2024-03-21 14:27:14.000000 djrender-0.1a11/djrender.egg-info/SOURCES.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-03-21 14:27:14.000000 djrender-0.1a11/djrender.egg-info/dependency_links.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-03-21 14:27:09.000000 djrender-0.1a11/djrender.egg-info/not-zip-safe
--rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-03-21 14:27:14.000000 djrender-0.1a11/djrender.egg-info/requires.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       13 2024-03-21 14:27:14.000000 djrender-0.1a11/djrender.egg-info/top_level.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-03-21 14:27:14.654393 djrender-0.1a11/setup.cfg
--rw-rw-r--   0 karl      (1000) karl      (1000)     1515 2024-03-21 14:27:03.000000 djrender-0.1a11/setup.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      104 2024-04-09 12:29:00.000000 djrender-0.1b1/MANIFEST.in
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-09 12:36:55.693416 djrender-0.1b1/PKG-INFO
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      468 2024-04-09 12:36:33.000000 djrender-0.1b1/django_render/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      343 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3247 2024-04-09 12:36:33.000000 djrender-0.1b1/django_render/decorators.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3235 2024-04-09 12:36:33.000000 djrender-0.1b1/django_render/response.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/static/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/static/django_render/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/static/django_render/fonts/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/static/django_render/fonts/.gitignore
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/static/django_render/images/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/static/django_render/images/.gitignore
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/static/django_render/js/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       17 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/static/django_render/js/.gitignore
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1754 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/telepath.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/templates/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/templates/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3497 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/templates/django_render/bootstrap.html
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/test/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       73 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      186 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3653 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/settings.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/test/tests/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/tests/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/urls.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/ui/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/ui/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3594 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/ui/forms.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1438 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/views.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/djrender.egg-info/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)      776 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/SOURCES.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/dependency_links.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-09 12:36:52.000000 djrender-0.1b1/djrender.egg-info/not-zip-safe
+-rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/requires.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/top_level.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-09 12:36:55.693416 djrender-0.1b1/setup.cfg
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1510 2024-04-09 12:36:33.000000 djrender-0.1b1/setup.py
```

### Comparing `djrender-0.1a11/PKG-INFO` & `djrender-0.1b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: djrender
-Version: 0.1a11
-Summary: A library for building frontends for Django with modern frameworks
+Version: 0.1b1
+Summary: A framework for building React frontends for Django projects
 Home-page: https://django-render.org
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://django-render.org/docs/
 Project-URL: Source, https://github.com/kaedroho/django-render/
 Project-URL: Tracker, https://github.com/kaedroho/django-render/issues
```

### Comparing `djrender-0.1a11/djangorender/decorators.py` & `djrender-0.1b1/django_render/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,42 +35,40 @@
                 # Response couldn't be converted into a Django Render response. Reload the page
                 return ReloadResponse()
 
         # Regular browser request
         # If the response is a Django Render response, wrap it in our bootstrap template
         # to load the React SPA and render the response data.
         if isinstance(response, BaseResponse):
-            if settings.DJREAM_VITE_BUNDLE_DIR:
+            VITE_BUNDLE_DIR = settings.DJANGO_RENDER.get("VITE_BUNDLE_DIR")
+            VITE_DEVSERVER_URL = settings.DJANGO_RENDER.get("VITE_DEVSERVER_URL")
+            if VITE_BUNDLE_DIR:
                 # Production - Use asset manifest to find URLs to bundled JS/CSS
                 asset_manifest = json.loads(
-                    (
-                        Path(settings.DJREAM_VITE_BUNDLE_DIR) / ".vite/manifest.json"
-                    ).read_text()
+                    (Path(VITE_BUNDLE_DIR) / ".vite/manifest.json").read_text()
                 )
 
                 js = [
                     static(asset_manifest["src/main.tsx"]["file"]),
                 ]
                 css = asset_manifest["src/main.tsx"]["css"]
                 vite_react_refresh_runtime = None
 
-            elif settings.DJREAM_VITE_DEVSERVER_URL:
+            elif VITE_DEVSERVER_URL:
                 # Development - Fetch JS/CSS from Vite server
                 js = [
-                    settings.DJREAM_VITE_DEVSERVER_URL + "/@vite/client",
-                    settings.DJREAM_VITE_DEVSERVER_URL + "/src/main.tsx",
+                    VITE_DEVSERVER_URL + "/@vite/client",
+                    VITE_DEVSERVER_URL + "/src/main.tsx",
                 ]
                 css = []
-                vite_react_refresh_runtime = (
-                    settings.DJREAM_VITE_DEVSERVER_URL + "/@react-refresh"
-                )
+                vite_react_refresh_runtime = VITE_DEVSERVER_URL + "/@react-refresh"
 
             else:
                 raise ImproperlyConfigured(
-                    "DJREAM_VITE_BUNDLE_DIR (production) or DJREAM_VITE_DEVSERVER_URL (development) must be set"
+                    "DJANGO_RENDER['VITE_BUNDLE_DIR'] (production) or DJANGO_RENDER['VITE_DEVSERVER_URL'] (development) must be set"
                 )
 
             # Wrap the response with our bootstrap template
             new_response = render(
                 request,
                 "djangorender/bootstrap.html",
                 {
```

### Comparing `djrender-0.1a11/djangorender/response.py` & `djrender-0.1b1/django_render/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 def get_messages(request):
     return [
         {
             "level": (
                 "error"
                 if message.level == messages.ERROR
-                else "warning" if message.level == messages.WARNING else "success"
+                else "warning"
+                if message.level == messages.WARNING
+                else "success"
             ),
             "html": conditional_escape(message.message),
         }
         for message in messages.get_messages(request)
     ]
 
 
@@ -68,15 +70,17 @@
         return {
             "view": view,
             "overlay": self.overlay,
             "title": self.title,
             "props": props,
             "context": {
                 name: import_string(provider)(self.request)
-                for name, provider in settings.DJREAM_CONTEXT_PROVIDERS.items()
+                for name, provider in settings.DJANGO_RENDER.get(
+                    "CONTEXT_PROVIDERS", {}
+                ).items()
             },
             "messages": get_messages(self.request),
         }
 
 
 class ReloadResponse(BaseResponse):
     """
```

### Comparing `djrender-0.1a11/djangorender/telepath.py` & `djrender-0.1b1/django_render/telepath.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1a11/djangorender/templates/djangorender/bootstrap.html` & `djrender-0.1b1/django_render/templates/django_render/bootstrap.html`

 * *Files identical despite different names*

### Comparing `djrender-0.1a11/djangorender/test/settings.py` & `djrender-0.1b1/django_render/test/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 ALLOWED_HOSTS = ["localhost", "testserver"]
 
 
 # Application definition
 
 INSTALLED_APPS = [
-    "djangorender",
-    "djangorender.test",
+    "django_render",
+    "django_render.test",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
     "django.contrib.sitemaps",
@@ -47,15 +47,15 @@
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
 ]
 
-ROOT_URLCONF = "djangorender.test.urls"
+ROOT_URLCONF = "django_render.test.urls"
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
         "DIRS": [],
         "APP_DIRS": True,
         "OPTIONS": {
```

### Comparing `djrender-0.1a11/djangorender/ui/forms.py` & `djrender-0.1b1/django_render/ui/forms.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1a11/djangorender/views.py` & `djrender-0.1b1/django_render/views.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1a11/djrender.egg-info/PKG-INFO` & `djrender-0.1b1/djrender.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: djrender
-Version: 0.1a11
-Summary: A library for building frontends for Django with modern frameworks
+Version: 0.1b1
+Summary: A framework for building React frontends for Django projects
 Home-page: https://django-render.org
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://django-render.org/docs/
 Project-URL: Source, https://github.com/kaedroho/django-render/
 Project-URL: Tracker, https://github.com/kaedroho/django-render/issues
```

### Comparing `djrender-0.1a11/djrender.egg-info/SOURCES.txt` & `djrender-0.1b1/djrender.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 MANIFEST.in
 setup.py
-djangorender/__init__.py
-djangorender/apps.py
-djangorender/decorators.py
-djangorender/response.py
-djangorender/telepath.py
-djangorender/views.py
-djangorender/static/djangorender/fonts/.gitignore
-djangorender/static/djangorender/images/.gitignore
-djangorender/static/djangorender/js/.gitignore
-djangorender/templates/djangorender/bootstrap.html
-djangorender/test/__init__.py
-djangorender/test/apps.py
-djangorender/test/settings.py
-djangorender/test/urls.py
-djangorender/test/tests/__init__.py
-djangorender/ui/__init__.py
-djangorender/ui/forms.py
+django_render/__init__.py
+django_render/apps.py
+django_render/decorators.py
+django_render/response.py
+django_render/telepath.py
+django_render/views.py
+django_render/static/django_render/fonts/.gitignore
+django_render/static/django_render/images/.gitignore
+django_render/static/django_render/js/.gitignore
+django_render/templates/django_render/bootstrap.html
+django_render/test/__init__.py
+django_render/test/apps.py
+django_render/test/settings.py
+django_render/test/urls.py
+django_render/test/tests/__init__.py
+django_render/ui/__init__.py
+django_render/ui/forms.py
 djrender.egg-info/PKG-INFO
 djrender.egg-info/SOURCES.txt
 djrender.egg-info/dependency_links.txt
 djrender.egg-info/not-zip-safe
 djrender.egg-info/requires.txt
 djrender.egg-info/top_level.txt
```

### Comparing `djrender-0.1a11/setup.py` & `djrender-0.1b1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 
 from os import path
 
-from djangorender import __version__
+from django_render import __version__
 from setuptools import find_packages, setup
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "../README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="djrender",
     version=__version__,
-    description="A library for building frontends for Django with modern frameworks",
+    description="A framework for building React frontends for Django projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Karl Hobley",
     author_email="karl@kaed.uk",
     url="https://django-render.org",
     project_urls={
         "Documentation": "https://django-render.org/docs/",
```

