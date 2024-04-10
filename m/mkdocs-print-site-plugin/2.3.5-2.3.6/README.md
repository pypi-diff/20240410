# Comparing `tmp/mkdocs-print-site-plugin-2.3.5.tar.gz` & `tmp/mkdocs-print-site-plugin-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-print-site-plugin-2.3.5.tar", last modified: Mon Jun 12 08:52:07 2023, max compression
+gzip compressed data, was "mkdocs-print-site-plugin-2.3.6.tar", last modified: Mon Aug 28 07:29:52 2023, max compression
```

## Comparing `mkdocs-print-site-plugin-2.3.5.tar` & `mkdocs-print-site-plugin-2.3.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.283180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-material.css
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-mkdocs.css
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site.css
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/js/print-site.js
--rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/cover_page.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/print_site_banner.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.283180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/test_building.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/test_exclude.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (999)     1064 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     3458 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2529 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (999)     3477 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
+-rw-r--r--   0 runner    (1001) docker     (999)     1286 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
+-rw-r--r--   0 runner    (1001) docker     (999)     1444 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
+-rw-r--r--   0 runner    (1001) docker     (999)     1568 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
+-rw-r--r--   0 runner    (1001) docker     (999)     1675 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
+-rw-r--r--   0 runner    (1001) docker     (999)     1789 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
+-rw-r--r--   0 runner    (1001) docker     (999)      738 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-material.css
+-rw-r--r--   0 runner    (1001) docker     (999)      949 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-mkdocs.css
+-rw-r--r--   0 runner    (1001) docker     (999)     5463 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site.css
+-rw-r--r--   0 runner    (1001) docker     (999)     1570 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (999)     4515 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/js/print-site.js
+-rw-r--r--   0 runner    (1001) docker     (999)    17119 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9147 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (999)      714 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/cover_page.tpl
+-rw-r--r--   0 runner    (1001) docker     (999)      557 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/print_site_banner.tpl
+-rw-r--r--   0 runner    (1001) docker     (999)     8832 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (999)      863 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3458 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1273 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       78 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       23 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1458 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9196 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/test_building.py
+-rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/test_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7564 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/test_urls.py
```

### Comparing `mkdocs-print-site-plugin-2.3.5/LICENSE` & `mkdocs-print-site-plugin-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/PKG-INFO` & `mkdocs-print-site-plugin-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.3.5
+Version: 2.3.6
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-print-site-plugin-2.3.5/README.md` & `mkdocs-print-site-plugin-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings1.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings1.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings2.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings2.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings3.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings3.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings4.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings4.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings5.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings5.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings6.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings6.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-material.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-material.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-mkdocs.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-mkdocs.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site.css` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/exclude.py` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/js/print-site.js` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/js/print-site.js`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/plugin.py` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,14 @@
 
         # Link to the PDF version of the entire site on a page.
         if self.config.get("path_to_pdf") != "":
             pdf_url = self.config.get("path_to_pdf")
             if is_external(pdf_url):
                 page.url_to_pdf = pdf_url
             else:
-                breakpoint()
                 page.url_to_pdf = get_relative_url(
                     pdf_url, page.file.url
                 )
 
         return html
 
     def on_page_context(self, context, page, config, nav, **kwargs):
@@ -281,15 +280,15 @@
         # print(f"\nName: {template_name}\nContext: {context.get('extra_css')}")
         if template_name == "404.html":
             self.context = context
             # Make sure paths are OK
             if config.get('extra_css'):
                 self.context['extra_css'] = [get_relative_url(f, self.print_page.file.url) for f in config.get('extra_css')]
             if config.get('extra_javascript'):
-                self.context['extra_javascript'] = [get_relative_url(f, self.print_page.file.url) for f in config.get('extra_javascript')]
+                self.context['extra_javascript'] = [get_relative_url(str(f), self.print_page.file.url) for f in config.get('extra_javascript')]
 
 
     def on_post_build(self, config, **kwargs):
         """
         The post_build event does not alter any variables. Use this event to call post-build scripts.
 
         See https://www.mkdocs.org/user-guide/plugins/#on_post_build.
```

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/renderer.py` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/cover_page.tpl` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/cover_page.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/print_site_banner.tpl` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/print_site_banner.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/urls.py` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/utils.py` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/PKG-INFO` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.3.5
+Version: 2.3.6
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/SOURCES.txt` & `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/setup.py` & `mkdocs-print-site-plugin-2.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = ""
     for line in f:
         long_description += line
 
 
 setup(
     name="mkdocs-print-site-plugin",
-    version="2.3.5",
+    version="2.3.6",
     description="MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin print pdf",
     url="https://github.com/timvink/mkdocs-print-site-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs-print-site-plugin-2.3.5/tests/test_building.py` & `mkdocs-print-site-plugin-2.3.6/tests/test_building.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.5/tests/test_urls.py` & `mkdocs-print-site-plugin-2.3.6/tests/test_urls.py`

 * *Files identical despite different names*

