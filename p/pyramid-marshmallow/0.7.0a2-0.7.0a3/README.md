# Comparing `tmp/pyramid-marshmallow-0.7.0a2.tar.gz` & `tmp/pyramid-marshmallow-0.7.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramid-marshmallow-0.7.0a2.tar", last modified: Tue Feb  1 23:55:45 2022, max compression
+gzip compressed data, was "pyramid-marshmallow-0.7.0a3.tar", last modified: Wed Apr 10 05:00:11 2024, max compression
```

## Comparing `pyramid-marshmallow-0.7.0a2.tar` & `pyramid-marshmallow-0.7.0a3.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 luhn       (501) staff       (20)        0 2022-02-01 23:55:45.946012 pyramid-marshmallow-0.7.0a2/
--rw-r--r--   0 luhn       (501) staff       (20)    10029 2022-02-01 23:55:45.946089 pyramid-marshmallow-0.7.0a2/PKG-INFO
--rw-r--r--   0 luhn       (501) staff       (20)     8826 2022-02-01 18:36:48.000000 pyramid-marshmallow-0.7.0a2/README.md
--rw-r--r--   0 luhn       (501) staff       (20)      261 2022-02-01 18:39:46.000000 pyramid-marshmallow-0.7.0a2/pyproject.toml
-drwxr-xr-x   0 luhn       (501) staff       (20)        0 2022-02-01 23:55:45.944658 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/
--rw-r--r--   0 luhn       (501) staff       (20)     1801 2022-02-01 18:36:48.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/__init__.py
-drwxr-xr-x   0 luhn       (501) staff       (20)        0 2022-02-01 23:55:45.945809 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/
--rw-r--r--   0 luhn       (501) staff       (20)     3343 2022-02-01 23:54:21.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/__init__.py
--rw-r--r--   0 luhn       (501) staff       (20)     2012 2022-02-01 18:36:48.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/generate.py
--rw-r--r--   0 luhn       (501) staff       (20)     2375 2022-02-01 18:36:48.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/serve.py
--rw-r--r--   0 luhn       (501) staff       (20)     8372 2022-02-01 23:44:26.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/spec.py
-drwxr-xr-x   0 luhn       (501) staff       (20)        0 2022-02-01 23:55:45.945353 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/
--rw-r--r--   0 luhn       (501) staff       (20)    10029 2022-02-01 23:55:45.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/PKG-INFO
--rw-r--r--   0 luhn       (501) staff       (20)      479 2022-02-01 23:55:45.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/SOURCES.txt
--rw-r--r--   0 luhn       (501) staff       (20)        1 2022-02-01 23:55:45.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/dependency_links.txt
--rw-r--r--   0 luhn       (501) staff       (20)      134 2022-02-01 23:55:45.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/entry_points.txt
--rw-r--r--   0 luhn       (501) staff       (20)      179 2022-02-01 23:55:45.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/requires.txt
--rw-r--r--   0 luhn       (501) staff       (20)       20 2022-02-01 23:55:45.000000 pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/top_level.txt
--rw-r--r--   0 luhn       (501) staff       (20)     1440 2022-02-01 23:55:45.946619 pyramid-marshmallow-0.7.0a2/setup.cfg
+drwxr-xr-x   0 luhn       (501) staff       (20)        0 2024-04-10 05:00:11.358239 pyramid-marshmallow-0.7.0a3/
+-rw-r--r--   0 luhn       (501) staff       (20)    10430 2024-04-10 05:00:11.358137 pyramid-marshmallow-0.7.0a3/PKG-INFO
+-rw-r--r--   0 luhn       (501) staff       (20)     8826 2022-02-01 18:36:48.000000 pyramid-marshmallow-0.7.0a3/README.md
+-rw-r--r--   0 luhn       (501) staff       (20)      261 2022-02-01 18:39:46.000000 pyramid-marshmallow-0.7.0a3/pyproject.toml
+drwxr-xr-x   0 luhn       (501) staff       (20)        0 2024-04-10 05:00:11.354048 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/
+-rw-r--r--   0 luhn       (501) staff       (20)     1924 2023-05-02 18:44:22.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/__init__.py
+drwxr-xr-x   0 luhn       (501) staff       (20)        0 2024-04-10 05:00:11.356099 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/
+-rw-r--r--   0 luhn       (501) staff       (20)     3365 2023-05-02 18:35:06.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/__init__.py
+-rw-r--r--   0 luhn       (501) staff       (20)     2012 2022-02-01 18:36:48.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/generate.py
+-rw-r--r--   0 luhn       (501) staff       (20)     2375 2022-02-01 18:36:48.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/serve.py
+-rw-r--r--   0 luhn       (501) staff       (20)     8574 2024-04-10 04:57:28.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/spec.py
+drwxr-xr-x   0 luhn       (501) staff       (20)        0 2024-04-10 05:00:11.357325 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/
+-rw-r--r--   0 luhn       (501) staff       (20)    10430 2024-04-10 05:00:11.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/PKG-INFO
+-rw-r--r--   0 luhn       (501) staff       (20)      572 2024-04-10 05:00:11.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/SOURCES.txt
+-rw-r--r--   0 luhn       (501) staff       (20)        1 2024-04-10 05:00:11.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/dependency_links.txt
+-rw-r--r--   0 luhn       (501) staff       (20)      133 2024-04-10 05:00:11.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/entry_points.txt
+-rw-r--r--   0 luhn       (501) staff       (20)      179 2024-04-10 05:00:11.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/requires.txt
+-rw-r--r--   0 luhn       (501) staff       (20)       20 2024-04-10 05:00:11.000000 pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/top_level.txt
+-rw-r--r--   0 luhn       (501) staff       (20)     1442 2024-04-10 05:00:11.358535 pyramid-marshmallow-0.7.0a3/setup.cfg
+drwxr-xr-x   0 luhn       (501) staff       (20)        0 2024-04-10 05:00:11.357119 pyramid-marshmallow-0.7.0a3/tests/
+-rw-r--r--   0 luhn       (501) staff       (20)     1623 2021-10-20 18:58:43.000000 pyramid-marshmallow-0.7.0a3/tests/test_general.py
+-rw-r--r--   0 luhn       (501) staff       (20)      930 2021-10-20 18:58:43.000000 pyramid-marshmallow-0.7.0a3/tests/test_integration.py
+-rw-r--r--   0 luhn       (501) staff       (20)     1167 2023-05-02 18:43:14.000000 pyramid-marshmallow-0.7.0a3/tests/test_marshal.py
+-rw-r--r--   0 luhn       (501) staff       (20)     2254 2021-10-20 18:58:43.000000 pyramid-marshmallow-0.7.0a3/tests/test_validate.py
```

### Comparing `pyramid-marshmallow-0.7.0a2/PKG-INFO` & `pyramid-marshmallow-0.7.0a3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: pyramid-marshmallow
-Version: 0.7.0a2
+Version: 0.7.0a3
 Summary: Validate request and response data with Marshmallow and optionally generate an OpenAPI spec.
 Home-page: https://github.com/luhn/pyramid-marshmallow
 Author: Theron Luhn
 Author-email: theron@luhn.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: pyramid>=1.7
+Requires-Dist: marshmallow~=3.0
+Requires-Dist: zope.interface>=3.8.0
 Provides-Extra: openapi
+Requires-Dist: apispec<7,>=3.0; extra == "openapi"
+Requires-Dist: PyYAML<7,>=5.4; extra == "openapi"
 Provides-Extra: testing
+Requires-Dist: pytest~=6.2; extra == "testing"
+Requires-Dist: webtest~=2.0; extra == "testing"
 Provides-Extra: linting
+Requires-Dist: black~=23.3; extra == "linting"
+Requires-Dist: flake8~=6.0.0; extra == "linting"
+Requires-Dist: isort~=5.12; extra == "linting"
 
 # pyramid-marshmallow
 
 pyramid-marshmallow is a simple Pyramid plugin that allows you to validate and marshal a JSON HTTP request or response using [Marshmallow](http://marshmallow.readthedocs.io/) schemas.
 You can then leverage this to automatically generate an OpenAPI specification for your API.
 
 > **Version 0.5 and greater requires Marshmallow 3.x.  For Marshmallow 2.x, use version 0.4.**
@@ -288,9 +296,7 @@
 
 [pyramid-apispec](https://pypi.org/project/pyramid-apispec/) allows you to augment view callable docstrings with OpenAPI definitions and can reference Marshmallow schemas with the apispec Marshmallow plugin.
 It does not support validating input and marshalling output.
 Schemas and routes must be manually declared.
 
 [Cornice](https://cornice.readthedocs.io/en/latest/schema.html#using-marshmallow) supports validation with Marshmallow schemas, however only on Cornice resources, not arbitrary Pyramid endpoints.
 It does not support auto-generating OpenAPI documentation.
-
-
```

### Comparing `pyramid-marshmallow-0.7.0a2/README.md` & `pyramid-marshmallow-0.7.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/__init__.py` & `pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from marshmallow import Schema, ValidationError
+from pyramid.response import Response
 from pyramid.viewderivers import VIEW
 
 __all__ = [
     "ValidationError",
 ]
 
 
@@ -62,15 +63,18 @@
 def view_marshaller(view, info):
     schema = process_schema(info.options.get("marshal"))
     if schema is None:
         return view
 
     def wrapped(context, request):
         output = view(context, request)
-        return schema.dump(output)
+        if isinstance(output, Response):
+            return output
+        else:
+            return schema.dump(output)
 
     return wrapped
 
 
 view_marshaller.options = ("marshal",)
```

### Comparing `pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/__init__.py` & `pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     """
 
     def __init__(self, registry):
         self.registry = registry
 
     def __call__(self, zone, merge):
-        return self._call(zone, tuple(merge))
+        return self._call(zone, tuple(merge) if merge else tuple())
 
     @functools.lru_cache
     def _call(self, zone, merge):
         return create_spec(self.registry, zone=zone, merge=merge)
 
 
 def _inject_params(view, zone=None, merge=None):
```

### Comparing `pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/generate.py` & `pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/generate.py`

 * *Files identical despite different names*

### Comparing `pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/serve.py` & `pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/serve.py`

 * *Files identical despite different names*

### Comparing `pyramid-marshmallow-0.7.0a2/pyramid_marshmallow/openapi/spec.py` & `pyramid-marshmallow-0.7.0a3/pyramid_marshmallow/openapi/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
     )
     spec = APISpec(
         title=title,
         version=version,
         openapi_version="3.0.2",
         plugins=[marshmallow_plugin],
     )
+    plugin_hook = registry.settings.get("openapi.plugin_hook")
+    if plugin_hook:
+        plugin_hook = name_resolver.maybe_resolve(plugin_hook)
+        plugin_hook(registry, spec, marshmallow_plugin)
     for path, operations in list_paths(registry.introspector):
         final_ops = dict()
         for method, view in operations.items():
             if zone is not None and zone != view.get("api_zone"):
                 continue
             summary, descr, user_op = split_docstring(view["callable"].__doc__)
             op = {
```

### Comparing `pyramid-marshmallow-0.7.0a2/pyramid_marshmallow.egg-info/PKG-INFO` & `pyramid-marshmallow-0.7.0a3/pyramid_marshmallow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: pyramid-marshmallow
-Version: 0.7.0a2
+Version: 0.7.0a3
 Summary: Validate request and response data with Marshmallow and optionally generate an OpenAPI spec.
 Home-page: https://github.com/luhn/pyramid-marshmallow
 Author: Theron Luhn
 Author-email: theron@luhn.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: pyramid>=1.7
+Requires-Dist: marshmallow~=3.0
+Requires-Dist: zope.interface>=3.8.0
 Provides-Extra: openapi
+Requires-Dist: apispec<7,>=3.0; extra == "openapi"
+Requires-Dist: PyYAML<7,>=5.4; extra == "openapi"
 Provides-Extra: testing
+Requires-Dist: pytest~=6.2; extra == "testing"
+Requires-Dist: webtest~=2.0; extra == "testing"
 Provides-Extra: linting
+Requires-Dist: black~=23.3; extra == "linting"
+Requires-Dist: flake8~=6.0.0; extra == "linting"
+Requires-Dist: isort~=5.12; extra == "linting"
 
 # pyramid-marshmallow
 
 pyramid-marshmallow is a simple Pyramid plugin that allows you to validate and marshal a JSON HTTP request or response using [Marshmallow](http://marshmallow.readthedocs.io/) schemas.
 You can then leverage this to automatically generate an OpenAPI specification for your API.
 
 > **Version 0.5 and greater requires Marshmallow 3.x.  For Marshmallow 2.x, use version 0.4.**
@@ -288,9 +296,7 @@
 
 [pyramid-apispec](https://pypi.org/project/pyramid-apispec/) allows you to augment view callable docstrings with OpenAPI definitions and can reference Marshmallow schemas with the apispec Marshmallow plugin.
 It does not support validating input and marshalling output.
 Schemas and routes must be manually declared.
 
 [Cornice](https://cornice.readthedocs.io/en/latest/schema.html#using-marshmallow) supports validation with Marshmallow schemas, however only on Cornice resources, not arbitrary Pyramid endpoints.
 It does not support auto-generating OpenAPI documentation.
-
-
```

### Comparing `pyramid-marshmallow-0.7.0a2/setup.cfg` & `pyramid-marshmallow-0.7.0a3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 [metadata]
 name = pyramid-marshmallow
-version = 0.7.0a2
+version = 0.7.0a3
 author = Theron Luhn
 author_email = theron@luhn.com
 description = Validate request and response data with Marshmallow and optionally generate an OpenAPI spec.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/luhn/pyramid-marshmallow
 classifiers = 
 	Development Status :: 3 - Alpha
 	Framework :: Pyramid
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Programming Language :: Python
 
 [options]
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	pyramid>=1.7
 	marshmallow~=3.0
 	zope.interface>=3.8.0
 
 [options.extras_require]
 openapi = 
-	apispec>=3.0,<6
+	apispec>=3.0,<7
 	PyYAML>=5.4,<7
 testing = 
 	pytest~=6.2
 	webtest~=2.0
 linting = 
-	black==22.1
-	flake8~=4.0.1
-	isort~=5.10
+	black~=23.3
+	flake8~=6.0.0
+	isort~=5.12
 
 [options.entry_points]
 console_scripts = 
 	generate-spec = pyramid_marshmallow.openapi.generate:generate
 	serve-spec = pyramid_marshmallow.openapi.serve:serve
 
 [egg_info]
```

