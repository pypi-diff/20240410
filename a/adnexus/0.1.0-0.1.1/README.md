# Comparing `tmp/adnexus-0.1.0.tar.gz` & `tmp/adnexus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adnexus-0.1.0.tar", max compression
+gzip compressed data, was "adnexus-0.1.1.tar", max compression
```

## Comparing `adnexus-0.1.0.tar` & `adnexus-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2024-04-10 09:49:37.166875 adnexus-0.1.0/LICENCE
--rw-r--r--   0        0        0     1950 2024-04-10 09:49:37.166875 adnexus-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/__init__.py
--rw-r--r--   0        0        0      537 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/config/__init__.py
--rw-r--r--   0        0        0      527 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/config/base_loader.py
--rw-r--r--   0        0        0      696 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/config/builtin.py
--rw-r--r--   0        0        0      219 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/config/helpers.py
--rw-r--r--   0        0        0     3809 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/containers.py
--rw-r--r--   0        0        0      668 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/decorators.py
--rw-r--r--   0        0        0      518 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/integrations/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/integrations/starlette.py
--rw-r--r--   0        0        0      172 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/markers.py
--rw-r--r--   0        0        0     2123 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/providers.py
--rw-r--r--   0        0        0     2680 2024-04-10 09:49:37.166875 adnexus-0.1.0/adnexus/wrappers.py
--rw-r--r--   0        0        0      965 2024-04-10 09:49:37.170874 adnexus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 adnexus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-10 09:58:25.321921 adnexus-0.1.1/LICENCE
+-rw-r--r--   0        0        0     1950 2024-04-10 09:58:25.321921 adnexus-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/__init__.py
+-rw-r--r--   0        0        0      537 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/__init__.py
+-rw-r--r--   0        0        0      527 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/base_loader.py
+-rw-r--r--   0        0        0      696 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/builtin.py
+-rw-r--r--   0        0        0      219 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/helpers.py
+-rw-r--r--   0        0        0     3809 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/containers.py
+-rw-r--r--   0        0        0      668 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/decorators.py
+-rw-r--r--   0        0        0      518 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/integrations/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/integrations/starlette.py
+-rw-r--r--   0        0        0      172 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/markers.py
+-rw-r--r--   0        0        0     2123 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/providers.py
+-rw-r--r--   0        0        0     2680 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/wrappers.py
+-rw-r--r--   0        0        0      969 2024-04-10 09:58:25.321921 adnexus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 adnexus-0.1.1/PKG-INFO
```

### Comparing `adnexus-0.1.0/LICENCE` & `adnexus-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/README.md` & `adnexus-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/config/__init__.py` & `adnexus-0.1.1/adnexus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/config/base_loader.py` & `adnexus-0.1.1/adnexus/config/base_loader.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/config/builtin.py` & `adnexus-0.1.1/adnexus/config/builtin.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/containers.py` & `adnexus-0.1.1/adnexus/containers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/decorators.py` & `adnexus-0.1.1/adnexus/decorators.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/exceptions.py` & `adnexus-0.1.1/adnexus/exceptions.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/integrations/starlette.py` & `adnexus-0.1.1/adnexus/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/providers.py` & `adnexus-0.1.1/adnexus/providers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/adnexus/wrappers.py` & `adnexus-0.1.1/adnexus/wrappers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.0/pyproject.toml` & `adnexus-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "adnexus"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [ "nl <nl@x-net.at>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.6.4"
@@ -36,11 +36,11 @@
 mkdocs-material = "^9.5.14"
 
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.3.5"
 
 [tool.coverage.run]
-source = ["xdi"]
+source = ["adnexus"]
 branch = false
 omit = ["*/integrations/*", "*/tests/*"]
```

### Comparing `adnexus-0.1.0/PKG-INFO` & `adnexus-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adnexus
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: nl
 Author-email: nl@x-net.at
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

