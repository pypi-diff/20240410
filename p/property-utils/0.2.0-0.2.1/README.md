# Comparing `tmp/property-utils-0.2.0.tar.gz` & `tmp/property-utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-utils-0.2.0.tar", last modified: Tue Apr  9 14:51:29 2024, max compression
+gzip compressed data, was "property-utils-0.2.1.tar", last modified: Wed Apr 10 16:05:49 2024, max compression
```

## Comparing `property-utils-0.2.0.tar` & `property-utils-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,39 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-09 14:51:29.947085 property-utils-0.2.0/
--rw-r--r--   0 max       (1000) max       (1000)     1076 2024-03-28 17:51:01.000000 property-utils-0.2.0/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-09 14:51:29.943751 property-utils-0.2.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     2907 2024-04-09 14:48:45.000000 property-utils-0.2.0/README.md
--rw-r--r--   0 max       (1000) max       (1000)     1535 2024-04-09 14:49:12.000000 property-utils-0.2.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-04-09 14:51:29.947085 property-utils-0.2.0/setup.cfg
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-09 14:51:29.943751 property-utils-0.2.0/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-09 14:51:29.943751 property-utils-0.2.0/src/property_utils/
--rw-r--r--   0 max       (1000) max       (1000)        0 2024-03-28 17:51:01.000000 property-utils-0.2.0/src/property_utils/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-09 14:51:29.943751 property-utils-0.2.0/src/property_utils.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-09 14:51:29.000000 property-utils-0.2.0/src/property_utils.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      272 2024-04-09 14:51:29.000000 property-utils-0.2.0/src/property_utils.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-04-09 14:51:29.000000 property-utils-0.2.0/src/property_utils.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       51 2024-04-09 14:51:29.000000 property-utils-0.2.0/src/property_utils.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)       15 2024-04-09 14:51:29.000000 property-utils-0.2.0/src/property_utils.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.784745 property-utils-0.2.1/
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2024-03-28 17:51:01.000000 property-utils-0.2.1/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-10 16:05:49.784745 property-utils-0.2.1/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     2907 2024-04-09 14:48:45.000000 property-utils-0.2.1/README.md
+-rw-r--r--   0 max       (1000) max       (1000)     1537 2024-04-10 16:05:33.000000 property-utils-0.2.1/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-04-10 16:05:49.784745 property-utils-0.2.1/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.774745 property-utils-0.2.1/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.774745 property-utils-0.2.1/src/property_utils/
+-rw-r--r--   0 max       (1000) max       (1000)        0 2024-03-28 17:51:01.000000 property-utils-0.2.1/src/property_utils/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.778078 property-utils-0.2.1/src/property_utils/constants/
+-rw-r--r--   0 max       (1000) max       (1000)       49 2024-04-08 13:07:09.000000 property-utils-0.2.1/src/property_utils/constants/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      898 2024-04-08 13:07:09.000000 property-utils-0.2.1/src/property_utils/constants/constants.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.778078 property-utils-0.2.1/src/property_utils/exceptions/
+-rw-r--r--   0 max       (1000) max       (1000)      142 2024-04-08 13:07:09.000000 property-utils-0.2.1/src/property_utils/exceptions/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      524 2024-03-28 17:51:01.000000 property-utils-0.2.1/src/property_utils/exceptions/base.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.778078 property-utils-0.2.1/src/property_utils/exceptions/properties/
+-rw-r--r--   0 max       (1000) max       (1000)      185 2024-04-08 13:07:09.000000 property-utils-0.2.1/src/property_utils/exceptions/properties/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      641 2024-03-28 17:51:01.000000 property-utils-0.2.1/src/property_utils/exceptions/properties/property.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.781412 property-utils-0.2.1/src/property_utils/exceptions/units/
+-rw-r--r--   0 max       (1000) max       (1000)      364 2024-04-08 13:07:09.000000 property-utils-0.2.1/src/property_utils/exceptions/units/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      866 2024-04-06 06:13:47.000000 property-utils-0.2.1/src/property_utils/exceptions/units/converter_types.py
+-rw-r--r--   0 max       (1000) max       (1000)      479 2024-03-28 17:51:01.000000 property-utils-0.2.1/src/property_utils/exceptions/units/descriptors.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.781412 property-utils-0.2.1/src/property_utils/properties/
+-rw-r--r--   0 max       (1000) max       (1000)      134 2024-04-08 13:07:09.000000 property-utils-0.2.1/src/property_utils/properties/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    28066 2024-04-09 14:48:45.000000 property-utils-0.2.1/src/property_utils/properties/property.py
+-rw-r--r--   0 max       (1000) max       (1000)     2794 2024-04-08 14:48:05.000000 property-utils-0.2.1/src/property_utils/properties/validated_property.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.781412 property-utils-0.2.1/src/property_utils/units/
+-rw-r--r--   0 max       (1000) max       (1000)       43 2024-04-08 13:07:09.000000 property-utils-0.2.1/src/property_utils/units/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2939 2024-04-08 15:23:31.000000 property-utils-0.2.1/src/property_utils/units/aliases.py
+-rw-r--r--   0 max       (1000) max       (1000)    33193 2024-04-08 14:48:05.000000 property-utils-0.2.1/src/property_utils/units/converter_types.py
+-rw-r--r--   0 max       (1000) max       (1000)    12051 2024-04-08 14:48:05.000000 property-utils-0.2.1/src/property_utils/units/converters.py
+-rw-r--r--   0 max       (1000) max       (1000)    67715 2024-04-08 14:48:05.000000 property-utils-0.2.1/src/property_utils/units/descriptors.py
+-rw-r--r--   0 max       (1000) max       (1000)     4383 2024-04-08 15:28:32.000000 property-utils-0.2.1/src/property_utils/units/units.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-10 16:05:49.781412 property-utils-0.2.1/src/property_utils.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-10 16:05:49.000000 property-utils-0.2.1/src/property_utils.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1061 2024-04-10 16:05:49.000000 property-utils-0.2.1/src/property_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-04-10 16:05:49.000000 property-utils-0.2.1/src/property_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       51 2024-04-10 16:05:49.000000 property-utils-0.2.1/src/property_utils.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)       15 2024-04-10 16:05:49.000000 property-utils-0.2.1/src/property_utils.egg-info/top_level.txt
```

### Comparing `property-utils-0.2.0/LICENSE` & `property-utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `property-utils-0.2.0/PKG-INFO` & `property-utils-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for programming that involves physical properties
 Author-email: Maximos Nikiforakis <nikiforos@live.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/Maxcode123/property-utils
 Project-URL: Issues, https://github.com/Maxcode123/property-utils/issues
 Keywords: physical properties,properties
 Classifier: Programming Language :: Python
```

### Comparing `property-utils-0.2.0/README.md` & `property-utils-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `property-utils-0.2.0/pyproject.toml` & `property-utils-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 line-length = 88
 
 [tool.mypy]
 exclude = "tests"
 
 [tool.setuptools.packages.find]
 where = ["src"]
-include = ["property_utils"]
-exclude = ["property_utils.tests"]
+include = ["property_utils*"]
+exclude = ["property_utils.tests*"]
 namespaces = false
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "property-utils"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="Maximos Nikiforakis", email="nikiforos@live.co.uk" },
 ]
 description = "Utilities for programming that involves physical properties"
 keywords = ["physical properties", "properties"]
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `property-utils-0.2.0/src/property_utils.egg-info/PKG-INFO` & `property-utils-0.2.1/src/property_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for programming that involves physical properties
 Author-email: Maximos Nikiforakis <nikiforos@live.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/Maxcode123/property-utils
 Project-URL: Issues, https://github.com/Maxcode123/property-utils/issues
 Keywords: physical properties,properties
 Classifier: Programming Language :: Python
```

