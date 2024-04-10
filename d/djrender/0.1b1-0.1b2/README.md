# Comparing `tmp/djrender-0.1b1.tar.gz` & `tmp/djrender-0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djrender-0.1b1.tar", last modified: Tue Apr  9 12:36:55 2024, max compression
+gzip compressed data, was "djrender-0.1b2.tar", last modified: Wed Apr 10 11:03:14 2024, max compression
```

## Comparing `djrender-0.1b1.tar` & `djrender-0.1b2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/
--rw-rw-r--   0 karl      (1000) karl      (1000)      104 2024-04-09 12:29:00.000000 djrender-0.1b1/MANIFEST.in
--rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-09 12:36:55.693416 djrender-0.1b1/PKG-INFO
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/
--rw-rw-r--   0 karl      (1000) karl      (1000)      468 2024-04-09 12:36:33.000000 djrender-0.1b1/django_render/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      343 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3247 2024-04-09 12:36:33.000000 djrender-0.1b1/django_render/decorators.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3235 2024-04-09 12:36:33.000000 djrender-0.1b1/django_render/response.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/static/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/static/django_render/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/static/django_render/fonts/
--rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/static/django_render/fonts/.gitignore
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/static/django_render/images/
--rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/static/django_render/images/.gitignore
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/static/django_render/js/
--rw-rw-r--   0 karl      (1000) karl      (1000)       17 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/static/django_render/js/.gitignore
--rw-rw-r--   0 karl      (1000) karl      (1000)     1754 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/telepath.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.689416 djrender-0.1b1/django_render/templates/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/templates/django_render/
--rw-rw-r--   0 karl      (1000) karl      (1000)     3497 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/templates/django_render/bootstrap.html
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/test/
--rw-rw-r--   0 karl      (1000) karl      (1000)       73 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      186 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3653 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/settings.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/test/tests/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/tests/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/test/urls.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/django_render/ui/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/ui/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3594 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/ui/forms.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1438 2024-04-09 12:29:00.000000 djrender-0.1b1/django_render/views.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-09 12:36:55.693416 djrender-0.1b1/djrender.egg-info/
--rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)      776 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/SOURCES.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/dependency_links.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-09 12:36:52.000000 djrender-0.1b1/djrender.egg-info/not-zip-safe
--rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/requires.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:36:55.000000 djrender-0.1b1/djrender.egg-info/top_level.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-09 12:36:55.693416 djrender-0.1b1/setup.cfg
--rw-rw-r--   0 karl      (1000) karl      (1000)     1510 2024-04-09 12:36:33.000000 djrender-0.1b1/setup.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.890696 djrender-0.1b2/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      104 2024-04-09 12:29:00.000000 djrender-0.1b2/MANIFEST.in
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-10 11:03:14.890696 djrender-0.1b2/PKG-INFO
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.882696 djrender-0.1b2/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      468 2024-04-10 11:02:58.000000 djrender-0.1b2/django_render/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      343 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3247 2024-04-09 12:36:33.000000 djrender-0.1b2/django_render/decorators.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3235 2024-04-09 12:36:33.000000 djrender-0.1b2/django_render/response.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.874696 djrender-0.1b2/django_render/static/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.874696 djrender-0.1b2/django_render/static/django_render/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.882696 djrender-0.1b2/django_render/static/django_render/fonts/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/static/django_render/fonts/.gitignore
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.882696 djrender-0.1b2/django_render/static/django_render/images/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/static/django_render/images/.gitignore
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.882696 djrender-0.1b2/django_render/static/django_render/js/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       17 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/static/django_render/js/.gitignore
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1754 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/telepath.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.874696 djrender-0.1b2/django_render/templates/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.882696 djrender-0.1b2/django_render/templates/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3507 2024-04-10 11:02:58.000000 djrender-0.1b2/django_render/templates/django_render/bootstrap.html
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.886696 djrender-0.1b2/django_render/test/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       73 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/test/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      186 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/test/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3653 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/test/settings.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.886696 djrender-0.1b2/django_render/test/tests/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/test/tests/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/test/urls.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.886696 djrender-0.1b2/django_render/ui/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/ui/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3594 2024-04-09 12:29:00.000000 djrender-0.1b2/django_render/ui/forms.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1430 2024-04-10 11:02:58.000000 djrender-0.1b2/django_render/views.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 11:03:14.890696 djrender-0.1b2/djrender.egg-info/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-10 11:03:14.000000 djrender-0.1b2/djrender.egg-info/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)      776 2024-04-10 11:03:14.000000 djrender-0.1b2/djrender.egg-info/SOURCES.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-10 11:03:14.000000 djrender-0.1b2/djrender.egg-info/dependency_links.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-09 12:36:52.000000 djrender-0.1b2/djrender.egg-info/not-zip-safe
+-rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-04-10 11:03:14.000000 djrender-0.1b2/djrender.egg-info/requires.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-10 11:03:14.000000 djrender-0.1b2/djrender.egg-info/top_level.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-10 11:03:14.890696 djrender-0.1b2/setup.cfg
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1510 2024-04-09 12:36:33.000000 djrender-0.1b2/setup.py
```

### Comparing `djrender-0.1b1/PKG-INFO` & `djrender-0.1b2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djrender
-Version: 0.1b1
+Version: 0.1b2
 Summary: A framework for building React frontends for Django projects
 Home-page: https://django-render.org
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://django-render.org/docs/
 Project-URL: Source, https://github.com/kaedroho/django-render/
```

### Comparing `djrender-0.1b1/django_render/decorators.py` & `djrender-0.1b2/django_render/decorators.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b1/django_render/response.py` & `djrender-0.1b2/django_render/response.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b1/django_render/telepath.py` & `djrender-0.1b2/django_render/telepath.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b1/django_render/templates/django_render/bootstrap.html` & `djrender-0.1b2/django_render/templates/django_render/bootstrap.html`

 * *Files 6% similar despite different names*

```diff
@@ -8,44 +8,44 @@
   <title>{% block title %}{% endblock %}</title>
 
   {% for src in css %}
   <link href="{% static src %}" rel="stylesheet" />
   {% endfor %}
   {% block loader_css %}
   <style>
-    .djangorender-load {
+    .django-render-load {
       position: absolute;
       left: 0;
       top: 0;
       width: 100%;
       height: 100%;
       z-index: 1000;
 
       opacity: 1;
       transition: opacity 0.2s;
     }
 
-    .djangorender-load--hidden {
+    .django-render-load--hidden {
       opacity: 0;
     }
 
-    .djangorender-load__spinner {
+    .django-render-load__spinner {
       opacity: 0;
       transition: opacity 0.2s;
 
       position: absolute;
       left: calc(50% - 40px);
       top: calc(50% - 40px)
     }
 
-    .djangorender-load--show-spinner .djangorender-load__spinner {
+    .django-render-load--show-spinner .django-render-load__spinner {
       opacity: 1;
     }
 
-    .djangorender-load__text {
+    .django-render-load__text {
       position: absolute;
       top: 32px;
       font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
       font-size: 13px;
       width: 80px;
       text-align: center;
     }
@@ -58,16 +58,16 @@
 
 <body>
   {% block noscript %}
   <noscript>You need to enable JavaScript to run this app.</noscript>
   {% endblock %}
 
   {% block loader %}
-  <div class="djangorender-load">
-    <div class="djangorender-load__spinner">
+  <div class="django-render-load">
+    <div class="django-render-load__spinner">
       <svg width="80" height="80" viewBox="0 0 200 200" color="#4c3fdd" fill="none" xmlns="http://www.w3.org/2000/svg">
         <defs>
           <linearGradient id="spinner-secondHalf">
             <stop offset="0%" stop-opacity="0" stop-color="currentColor" />
             <stop offset="100%" stop-opacity="0.5" stop-color="currentColor" />
           </linearGradient>
           <linearGradient id="spinner-firstHalf">
@@ -104,14 +104,14 @@
     window.__vite_plugin_react_preamble_installed__ = true
   </script>
   {% endif %}
   {% for src in js %}
   <script type="module" src="{{ src }}" async defer></script>
   {% endfor %}
   {% block loader_js %}
-  <script>document.addEventListener('DOMContentLoaded', () => { setTimeout(() => { document.querySelector('.djangorender-load').classList.add('djangorender-load--show-spinner') }, 100) });</script>
+  <script>document.addEventListener('DOMContentLoaded', () => { setTimeout(() => { document.querySelector('.django-render-load').classList.add('django-render-load--show-spinner') }, 100) });</script>
   {% endblock %}
   {% block extra_body %}
   {% endblock %}
 </body>
 
 </html>
```

### Comparing `djrender-0.1b1/django_render/test/settings.py` & `djrender-0.1b2/django_render/test/settings.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b1/django_render/ui/forms.py` & `djrender-0.1b2/django_render/ui/forms.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b1/django_render/views.py` & `djrender-0.1b2/django_render/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
         Pass response_kwargs to the constructor of the response class.
         """
         return self.response_class(
             self.request,
             self.view_name,
             props,
-            supported_modes=self.overlay,
+            overlay=self.overlay,
             title=self.title,
         )
 
 
-class djangorenderView(ResponseMixin, ContextMixin, View):
+class DjangoRenderView(ResponseMixin, ContextMixin, View):
     """
     Render a djangorender view. Pass keyword arguments from the URLconf to the context.
     """
 
     @method_decorator(djangorender_view)
     def dispatch(self, request, *args, **kwargs):
         return super().dispatch(request, *args, **kwargs)
```

### Comparing `djrender-0.1b1/djrender.egg-info/PKG-INFO` & `djrender-0.1b2/djrender.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djrender
-Version: 0.1b1
+Version: 0.1b2
 Summary: A framework for building React frontends for Django projects
 Home-page: https://django-render.org
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://django-render.org/docs/
 Project-URL: Source, https://github.com/kaedroho/django-render/
```

### Comparing `djrender-0.1b1/djrender.egg-info/SOURCES.txt` & `djrender-0.1b2/djrender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djrender-0.1b1/setup.py` & `djrender-0.1b2/setup.py`

 * *Files identical despite different names*

