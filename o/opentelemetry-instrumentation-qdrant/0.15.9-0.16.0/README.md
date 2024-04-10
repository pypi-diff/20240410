# Comparing `tmp/opentelemetry_instrumentation_qdrant-0.15.9.tar.gz` & `tmp/opentelemetry_instrumentation_qdrant-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.15.9.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.16.0.tar", max compression
```

## Comparing `opentelemetry_instrumentation_qdrant-0.15.9.tar` & `opentelemetry_instrumentation_qdrant-0.16.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      572 2024-04-03 18:13:50.329438 opentelemetry_instrumentation_qdrant-0.15.9/README.md
--rw-r--r--   0        0        0     1925 2024-04-03 18:13:50.329438 opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     2943 2024-04-03 18:13:50.329438 opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
--rw-r--r--   0        0        0     2828 2024-04-03 18:13:50.329438 opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
--rw-r--r--   0        0        0       23 2024-04-03 18:13:50.329438 opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/version.py
--rw-r--r--   0        0        0     3657 2024-04-03 18:13:50.329438 opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/wrapper.py
--rw-r--r--   0        0        0     1352 2024-04-03 18:14:27.145462 opentelemetry_instrumentation_qdrant-0.15.9/pyproject.toml
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.15.9/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-04-10 02:22:16.978129 opentelemetry_instrumentation_qdrant-0.16.0/README.md
+-rw-r--r--   0        0        0     1925 2024-04-10 02:22:16.978129 opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-10 02:22:16.978129 opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
+-rw-r--r--   0        0        0     2828 2024-04-10 02:22:16.978129 opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
+-rw-r--r--   0        0        0       23 2024-04-10 02:22:16.978129 opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/version.py
+-rw-r--r--   0        0        0     3657 2024-04-10 02:22:16.978129 opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/wrapper.py
+-rw-r--r--   0        0        0     1352 2024-04-10 02:22:45.494434 opentelemetry_instrumentation_qdrant-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.16.0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_qdrant-0.15.9/README.md` & `opentelemetry_instrumentation_qdrant-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/__init__.py` & `opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.9/opentelemetry/instrumentation/qdrant/wrapper.py` & `opentelemetry_instrumentation_qdrant-0.16.0/opentelemetry/instrumentation/qdrant/wrapper.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.9/pyproject.toml` & `opentelemetry_instrumentation_qdrant-0.16.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-qdrant"
-version = "0.15.9"
+version = "0.16.0"
 description = "OpenTelemetry Qdrant instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant"
@@ -31,15 +31,15 @@
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "2.1.0"
 flake8 = "7.0.0"
 
 [tool.poetry.group.test.dependencies]
 qdrant-client = "^1.7.3"
-pytest = "8.1.0"
+pytest = "8.1.1"
 pytest-sugar = "1.0.0"
 opentelemetry-sdk = "^1.23.0"
 
 [build-system]
 requires = [ "poetry-core" ]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `opentelemetry_instrumentation_qdrant-0.15.9/PKG-INFO` & `opentelemetry_instrumentation_qdrant-0.16.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-qdrant
-Version: 0.15.9
+Version: 0.16.0
 Summary: OpenTelemetry Qdrant instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-qdrant Version:
-0.15.9 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
+0.16.0 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-qdrant License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

