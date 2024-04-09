# Comparing `tmp/alliance_platform_codegen-0.0.1.tar.gz` & `tmp/alliance_platform_codegen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_codegen-0.0.1.tar", last modified: Tue Apr  9 10:48:00 2024, max compression
+gzip compressed data, was "alliance_platform_codegen-0.0.2.tar", last modified: Tue Apr  9 23:43:29 2024, max compression
```

## Comparing `alliance_platform_codegen-0.0.1.tar` & `alliance_platform_codegen-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/post_processors/__init__.py
--rw-r--r--   0        0        0     3587 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/post_processors/js.py
--rw-r--r--   0        0        0    15716 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/printer.py
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/py.typed
--rw-r--r--   0        0        0     6352 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/registry.py
--rw-r--r--   0        0        0     1332 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/settings.py
--rw-r--r--   0        0        0    18618 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/alliance_platform/codegen/typescript.py
--rw-r--r--   0        0        0      848 2024-04-09 10:48:00.323068 alliance_platform_codegen-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    14091 2024-04-09 10:47:27.171190 alliance_platform_codegen-0.0.1/tests/test_printer.py
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 alliance_platform_codegen-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 23:43:00.532542 alliance_platform_codegen-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/apps.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/post_processors/__init__.py
+-rw-r--r--   0        0        0     3587 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/post_processors/js.py
+-rw-r--r--   0        0        0    15716 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/printer.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/py.typed
+-rw-r--r--   0        0        0     6352 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/registry.py
+-rw-r--r--   0        0        0     1332 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/settings.py
+-rw-r--r--   0        0        0    18618 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/alliance_platform/codegen/typescript.py
+-rw-r--r--   0        0        0      848 2024-04-09 23:43:29.716855 alliance_platform_codegen-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    14091 2024-04-09 23:43:00.536542 alliance_platform_codegen-0.0.2/tests/test_printer.py
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 alliance_platform_codegen-0.0.2/PKG-INFO
```

### Comparing `alliance_platform_codegen-0.0.1/alliance_platform/codegen/post_processors/js.py` & `alliance_platform_codegen-0.0.2/alliance_platform/codegen/post_processors/js.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_codegen-0.0.1/alliance_platform/codegen/printer.py` & `alliance_platform_codegen-0.0.2/alliance_platform/codegen/printer.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_codegen-0.0.1/alliance_platform/codegen/registry.py` & `alliance_platform_codegen-0.0.2/alliance_platform/codegen/registry.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_codegen-0.0.1/alliance_platform/codegen/settings.py` & `alliance_platform_codegen-0.0.2/alliance_platform/codegen/settings.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_codegen-0.0.1/alliance_platform/codegen/typescript.py` & `alliance_platform_codegen-0.0.2/alliance_platform/codegen/typescript.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_codegen-0.0.1/pyproject.toml` & `alliance_platform_codegen-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "alliance-platform-core",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 include = [
     "alliance_platform/codegen/py.typed",
 ]
-version = "0.0.1"
+version = "0.0.2"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `alliance_platform_codegen-0.0.1/tests/test_printer.py` & `alliance_platform_codegen-0.0.2/tests/test_printer.py`

 * *Files identical despite different names*

