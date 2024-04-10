# Comparing `tmp/adnexus-0.1.3.tar.gz` & `tmp/adnexus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adnexus-0.1.3.tar", max compression
+gzip compressed data, was "adnexus-0.1.4.tar", max compression
```

## Comparing `adnexus-0.1.3.tar` & `adnexus-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2024-04-10 11:18:43.531823 adnexus-0.1.3/LICENCE
--rw-r--r--   0        0        0     2197 2024-04-10 11:18:43.531823 adnexus-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-10 11:18:43.531823 adnexus-0.1.3/adnexus/__init__.py
--rw-r--r--   0        0        0      537 2024-04-10 11:18:43.531823 adnexus-0.1.3/adnexus/config/__init__.py
--rw-r--r--   0        0        0      527 2024-04-10 11:18:43.531823 adnexus-0.1.3/adnexus/config/base_loader.py
--rw-r--r--   0        0        0      696 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/config/builtin.py
--rw-r--r--   0        0        0      219 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/config/helpers.py
--rw-r--r--   0        0        0     3809 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/containers.py
--rw-r--r--   0        0        0      668 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/decorators.py
--rw-r--r--   0        0        0      518 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/integrations/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/integrations/starlette.py
--rw-r--r--   0        0        0      172 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/markers.py
--rw-r--r--   0        0        0     2123 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/providers.py
--rw-r--r--   0        0        0     2680 2024-04-10 11:18:43.535823 adnexus-0.1.3/adnexus/wrappers.py
--rw-r--r--   0        0        0     1074 2024-04-10 11:18:43.535823 adnexus-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 adnexus-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-10 11:51:45.021406 adnexus-0.1.4/LICENCE
+-rw-r--r--   0        0        0     2213 2024-04-10 11:51:45.021406 adnexus-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/__init__.py
+-rw-r--r--   0        0        0      537 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/config/__init__.py
+-rw-r--r--   0        0        0      527 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/config/base_loader.py
+-rw-r--r--   0        0        0      696 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/config/builtin.py
+-rw-r--r--   0        0        0      219 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/config/helpers.py
+-rw-r--r--   0        0        0     3809 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/containers.py
+-rw-r--r--   0        0        0      668 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/decorators.py
+-rw-r--r--   0        0        0      518 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/integrations/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/integrations/starlette.py
+-rw-r--r--   0        0        0      172 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/markers.py
+-rw-r--r--   0        0        0     2123 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/providers.py
+-rw-r--r--   0        0        0     2680 2024-04-10 11:51:45.021406 adnexus-0.1.4/adnexus/wrappers.py
+-rw-r--r--   0        0        0     1074 2024-04-10 11:51:45.025406 adnexus-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 adnexus-0.1.4/PKG-INFO
```

### Comparing `adnexus-0.1.3/LICENCE` & `adnexus-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/README.md` & `adnexus-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![tests](https://github.com/Nictec/XDI/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/XDI/actions/workflows/main.yml) [![docs](https://github.com/Nictec/adnexus/actions/workflows/docs.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/docs.yml) [![build](https://github.com/Nictec/adnexus/actions/workflows/build.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/build.yml)
-# XDI Framework
-**XDI is a modern and declarative DI and IoC framework using pydantic for config and data.**
+[![tests](https://github.com/Nictec/Adnexus/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/Adnexus/actions/workflows/main.yml) [![docs](https://github.com/Nictec/adnexus/actions/workflows/docs.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/docs.yml) [![build](https://github.com/Nictec/adnexus/actions/workflows/build.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/build.yml)
+# Adnexus Framework
+**Adnexus is a modern and declarative DI and IoC framework using pydantic for config and data.**
 
 ## Key features
 
 - **Fast:** Very high performance thanks to pydantic and preemptive wiring
 - **Developer friendly:** Declarative Container definition to take the "Magic" out of DI
 - **Good compatibility:** Can be used with almost every framework and supports async
```

### Comparing `adnexus-0.1.3/adnexus/config/__init__.py` & `adnexus-0.1.4/adnexus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/config/base_loader.py` & `adnexus-0.1.4/adnexus/config/base_loader.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/config/builtin.py` & `adnexus-0.1.4/adnexus/config/builtin.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/containers.py` & `adnexus-0.1.4/adnexus/containers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/decorators.py` & `adnexus-0.1.4/adnexus/decorators.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/exceptions.py` & `adnexus-0.1.4/adnexus/exceptions.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/integrations/starlette.py` & `adnexus-0.1.4/adnexus/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/providers.py` & `adnexus-0.1.4/adnexus/providers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/adnexus/wrappers.py` & `adnexus-0.1.4/adnexus/wrappers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.3/pyproject.toml` & `adnexus-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "adnexus"
-version = "0.1.3"
+version = "0.1.4"
 description = "Modern and fully typed declarative Di and IoC Framework"
 authors = [ "nl <nl@x-net.at>",]
 readme = "README.md"
 repository = "https://github.com/Nictec/adnexus/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `adnexus-0.1.3/PKG-INFO` & `adnexus-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: adnexus
-Version: 0.1.3
+Version: 0.1.4
 Summary: Modern and fully typed declarative Di and IoC Framework
 Home-page: https://github.com/Nictec/adnexus/
 Author: nl
 Author-email: nl@x-net.at
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Project-URL: Repository, https://github.com/Nictec/adnexus/
 Description-Content-Type: text/markdown
 
-[![tests](https://github.com/Nictec/XDI/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/XDI/actions/workflows/main.yml) [![docs](https://github.com/Nictec/adnexus/actions/workflows/docs.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/docs.yml) [![build](https://github.com/Nictec/adnexus/actions/workflows/build.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/build.yml)
-# XDI Framework
-**XDI is a modern and declarative DI and IoC framework using pydantic for config and data.**
+[![tests](https://github.com/Nictec/Adnexus/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/Adnexus/actions/workflows/main.yml) [![docs](https://github.com/Nictec/adnexus/actions/workflows/docs.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/docs.yml) [![build](https://github.com/Nictec/adnexus/actions/workflows/build.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/build.yml)
+# Adnexus Framework
+**Adnexus is a modern and declarative DI and IoC framework using pydantic for config and data.**
 
 ## Key features
 
 - **Fast:** Very high performance thanks to pydantic and preemptive wiring
 - **Developer friendly:** Declarative Container definition to take the "Magic" out of DI
 - **Good compatibility:** Can be used with almost every framework and supports async
```

