# Comparing `tmp/alliance_platform_frontend-0.0.1.tar.gz` & `tmp/alliance_platform_frontend-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_frontend-0.0.1.tar", last modified: Tue Apr  9 10:47:55 2024, max compression
+gzip compressed data, was "alliance_platform_frontend-0.0.2.tar", last modified: Wed Apr 10 00:56:57 2024, max compression
```

## Comparing `alliance_platform_frontend-0.0.1.tar` & `alliance_platform_frontend-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2944 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/README.md
--rw-r--r--   0        0        0       22 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/__init__.py
--rw-r--r--   0        0        0      784 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/button.py
--rw-r--r--   0        0        0     1839 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/date_picker.py
--rw-r--r--   0        0        0     2524 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/icon.py
--rw-r--r--   0        0        0     1421 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/inline_alert.py
--rw-r--r--   0        0        0     1464 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/menubar.py
--rw-r--r--   0        0        0     2075 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/misc.py
--rw-r--r--   0        0        0     1622 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/pagination.py
--rw-r--r--   0        0        0     2270 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/table.py
--rw-r--r--   0        0        0     1127 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/time_input.py
--rw-r--r--   0        0        0     1243 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/utils.py
--rw-r--r--   0        0        0      357 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/apps.py
--rw-r--r--   0        0        0      512 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/__init__.py
--rw-r--r--   0        0        0     3310 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/asset_registry.py
--rw-r--r--   0        0        0    15999 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/base.py
--rw-r--r--   0        0        0    17174 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/context.py
--rw-r--r--   0        0        0     2507 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/middleware.py
--rw-r--r--   0        0        0    13537 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/ssr.py
--rw-r--r--   0        0        0     7051 2024-04-09 10:47:27.171190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/vanilla_extract.py
--rw-r--r--   0        0        0    33406 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/vite.py
--rw-r--r--   0        0        0      175 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/vitePreload.ts
--rw-r--r--   0        0        0    11144 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/dom_possible_standard_names.py
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/forms/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/forms/renderers.py
--rw-r--r--   0        0        0     5266 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/management/commands/extract_frontend_assets.py
--rw-r--r--   0        0        0    10434 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/prop_handlers.py
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/py.typed
--rw-r--r--   0        0        0     3867 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/settings.py
--rw-r--r--   0        0        0     2684 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/templates/bundler_dev_check.html
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/__init__.py
--rw-r--r--   0        0        0     5451 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/alliance_ui.py
--rw-r--r--   0        0        0    12851 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/bundler.py
--rw-r--r--   0        0        0     9664 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/form.py
--rw-r--r--   0        0        0    56265 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/react.py
--rw-r--r--   0        0        0     4316 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/vanilla_extract.py
--rw-r--r--   0        0        0     3283 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/alliance_platform/frontend/util.py
--rw-r--r--   0        0        0     2120 2024-04-09 10:47:55.059091 alliance_platform_frontend-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2503 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/fixtures/build_test/manifest.json
--rw-r--r--   0        0        0       39 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/fixtures/development-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0       30 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/fixtures/production-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0      648 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/fixtures/server_build_test/manifest.json
--rw-r--r--   0        0        0     7955 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/test_alliance_ui_templatetags.py
--rw-r--r--   0        0        0    11119 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/test_bundler.py
--rw-r--r--   0        0        0    33736 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/test_bundler_templatetags.py
--rw-r--r--   0        0        0     5837 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/test_context.py
--rw-r--r--   0        0        0      721 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-09 10:47:27.175190 alliance_platform_frontend-0.0.1/tests/test_utils/bundler.py
--rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2946 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/button.py
+-rw-r--r--   0        0        0     1839 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/date_picker.py
+-rw-r--r--   0        0        0     2524 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/icon.py
+-rw-r--r--   0        0        0     1421 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/inline_alert.py
+-rw-r--r--   0        0        0     1464 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/menubar.py
+-rw-r--r--   0        0        0     2075 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/misc.py
+-rw-r--r--   0        0        0     1622 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/pagination.py
+-rw-r--r--   0        0        0     2270 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/table.py
+-rw-r--r--   0        0        0     1127 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/time_input.py
+-rw-r--r--   0        0        0     1243 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/utils.py
+-rw-r--r--   0        0        0      358 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/apps.py
+-rw-r--r--   0        0        0      512 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/__init__.py
+-rw-r--r--   0        0        0     3310 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/asset_registry.py
+-rw-r--r--   0        0        0    15999 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/base.py
+-rw-r--r--   0        0        0    17174 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/context.py
+-rw-r--r--   0        0        0     2507 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/middleware.py
+-rw-r--r--   0        0        0    13537 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/ssr.py
+-rw-r--r--   0        0        0     7051 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vanilla_extract.py
+-rw-r--r--   0        0        0    33406 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vite.py
+-rw-r--r--   0        0        0      175 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vitePreload.ts
+-rw-r--r--   0        0        0    11144 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/dom_possible_standard_names.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/forms/__init__.py
+-rw-r--r--   0        0        0     1620 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/forms/renderers.py
+-rw-r--r--   0        0        0     5266 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/management/commands/extract_frontend_assets.py
+-rw-r--r--   0        0        0    10434 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/prop_handlers.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/py.typed
+-rw-r--r--   0        0        0     3867 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/settings.py
+-rw-r--r--   0        0        0     2684 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templates/bundler_dev_check.html
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/__init__.py
+-rw-r--r--   0        0        0     5451 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/alliance_ui.py
+-rw-r--r--   0        0        0    12851 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/bundler.py
+-rw-r--r--   0        0        0     9664 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/form.py
+-rw-r--r--   0        0        0    56265 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/react.py
+-rw-r--r--   0        0        0     4316 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/vanilla_extract.py
+-rw-r--r--   0        0        0     3283 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/util.py
+-rw-r--r--   0        0        0     2120 2024-04-10 00:56:57.919972 alliance_platform_frontend-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2503 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/tests/fixtures/build_test/manifest.json
+-rw-r--r--   0        0        0       39 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/tests/fixtures/development-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0       30 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/fixtures/production-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0      648 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/fixtures/server_build_test/manifest.json
+-rw-r--r--   0        0        0     7955 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_alliance_ui_templatetags.py
+-rw-r--r--   0        0        0    11119 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_bundler.py
+-rw-r--r--   0        0        0    33736 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_bundler_templatetags.py
+-rw-r--r--   0        0        0     5837 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_context.py
+-rw-r--r--   0        0        0      721 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_utils/bundler.py
+-rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.2/PKG-INFO
```

### Comparing `alliance_platform_frontend-0.0.1/README.md` & `alliance_platform_frontend-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     * [Bundler](#bundler)
     * [Templates](#templates)
     * [Template Tags](#template-tags)
 * [Release](#release-process)
 
 ## Installation
 
-`pip install alliance-django-frontend`
+`pip install alliance-platform-frontend`
 
 ## System Requirements
 
 * Supports django 4.2 and 5.0
 * Python >=3.11
 
 ## Usage
```

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/button.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/button.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/date_picker.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/date_picker.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/icon.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/icon.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/inline_alert.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/inline_alert.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/menubar.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/menubar.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/misc.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/misc.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/pagination.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/pagination.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/table.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/table.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/time_input.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/time_input.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/alliance_ui/utils.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/utils.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/__init__.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/asset_registry.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/asset_registry.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/base.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/base.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/context.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/middleware.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/middleware.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/ssr.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/ssr.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/vanilla_extract.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/bundler/vite.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vite.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/dom_possible_standard_names.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/dom_possible_standard_names.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/forms/renderers.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/management/commands/extract_frontend_assets.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/management/commands/extract_frontend_assets.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/prop_handlers.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/prop_handlers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/settings.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/settings.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/templates/bundler_dev_check.html` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templates/bundler_dev_check.html`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/alliance_ui.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/alliance_ui.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/bundler.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/form.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/react.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/react.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/templatetags/vanilla_extract.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/alliance_platform/frontend/util.py` & `alliance_platform_frontend-0.0.2/alliance_platform/frontend/util.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/pyproject.toml` & `alliance_platform_frontend-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 include = [
     "alliance_platform/frontend/py.typed",
 ]
-version = "0.0.1"
+version = "0.0.2"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [project.urls]
 issues = "https://github.com/AllianceSoftware/alliance-platform-py/issues"
 homepage = "https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend"
```

### Comparing `alliance_platform_frontend-0.0.1/tests/fixtures/build_test/manifest.json` & `alliance_platform_frontend-0.0.2/tests/fixtures/build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/tests/fixtures/server_build_test/manifest.json` & `alliance_platform_frontend-0.0.2/tests/fixtures/server_build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/tests/test_alliance_ui_templatetags.py` & `alliance_platform_frontend-0.0.2/tests/test_alliance_ui_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/tests/test_bundler.py` & `alliance_platform_frontend-0.0.2/tests/test_bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/tests/test_bundler_templatetags.py` & `alliance_platform_frontend-0.0.2/tests/test_bundler_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/tests/test_context.py` & `alliance_platform_frontend-0.0.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/tests/test_utils/__init__.py` & `alliance_platform_frontend-0.0.2/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/tests/test_utils/bundler.py` & `alliance_platform_frontend-0.0.2/tests/test_utils/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.1/PKG-INFO` & `alliance_platform_frontend-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alliance-platform-frontend
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django integration for Frontend Bundlers & React
 Keywords: django alliance alliancesoftware
 Home-page: https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend
 Author-Email: Alliance Software <support@alliancesoftware.com.au>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -43,15 +43,15 @@
     * [Bundler](#bundler)
     * [Templates](#templates)
     * [Template Tags](#template-tags)
 * [Release](#release-process)
 
 ## Installation
 
-`pip install alliance-django-frontend`
+`pip install alliance-platform-frontend`
 
 ## System Requirements
 
 * Supports django 4.2 and 5.0
 * Python >=3.11
 
 ## Usage
```

