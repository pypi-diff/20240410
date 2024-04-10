# Comparing `tmp/azure-functions-extension-base-1.0.0a5.tar.gz` & `tmp/azure-functions-extension-base-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-functions-extension-base-1.0.0a5.tar", last modified: Mon Apr  8 17:04:11 2024, max compression
+gzip compressed data, was "azure-functions-extension-base-1.0.0a6.tar", last modified: Wed Apr 10 01:39:43 2024, max compression
```

## Comparing `azure-functions-extension-base-1.0.0a5.tar` & `azure-functions-extension-base-1.0.0a6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.705120 azure-functions-extension-base-1.0.0a5/
--rw-rw-rw-   0        0        0     1093 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/LICENSE
--rw-rw-rw-   0        0        0       91 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/MANIFEST.in
--rw-rw-rw-   0        0        0     1497 2024-04-08 17:04:11.697897 azure-functions-extension-base-1.0.0a5/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-03-27 18:57:52.000000 azure-functions-extension-base-1.0.0a5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.514428 azure-functions-extension-base-1.0.0a5/azure/
--rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/azure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.529333 azure-functions-extension-base-1.0.0a5/azure/functions/
--rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/azure/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.547929 azure-functions-extension-base-1.0.0a5/azure/functions/extension/
--rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.588046 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/
--rw-rw-rw-   0        0        0      856 2024-04-08 17:02:01.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/__init__.py
--rw-rw-rw-   0        0        0     5760 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/meta.py
--rw-rw-rw-   0        0        0      296 2024-03-27 18:57:52.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/sdkType.py
--rw-rw-rw-   0        0        0     9064 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/utils.py
--rw-rw-rw-   0        0        0     5071 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/web.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.686770 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/
--rw-rw-rw-   0        0        0     1497 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1405 2024-03-27 14:46:39.000000 azure-functions-extension-base-1.0.0a5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 17:04:11.707260 azure-functions-extension-base-1.0.0a5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.678633 azure-functions-extension-base-1.0.0a5/tests/
--rw-rw-rw-   0        0        0      519 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/tests/__init__.py
--rw-rw-rw-   0        0        0    11527 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/tests/test_meta.py
--rw-rw-rw-   0        0        0      656 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/tests/test_sdk_type.py
--rw-rw-rw-   0        0        0    12756 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/tests/test_utils.py
--rw-rw-rw-   0        0        0    15462 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/tests/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:39:43.365220 azure-functions-extension-base-1.0.0a6/
+-rw-rw-rw-   0        0        0     1093 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1497 2024-04-10 01:39:43.365220 azure-functions-extension-base-1.0.0a6/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 01:39:43.304845 azure-functions-extension-base-1.0.0a6/azure/
+-rw-rw-rw-   0        0        0       66 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/azure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:39:43.304845 azure-functions-extension-base-1.0.0a6/azure/functions/
+-rw-rw-rw-   0        0        0       66 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/azure/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:39:43.304845 azure-functions-extension-base-1.0.0a6/azure/functions/extension/
+-rw-rw-rw-   0        0        0       66 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/azure/functions/extension/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:39:43.316925 azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/
+-rw-rw-rw-   0        0        0      856 2024-04-10 01:38:49.000000 azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/__init__.py
+-rw-rw-rw-   0        0        0     5760 2024-04-10 01:38:49.000000 azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/meta.py
+-rw-rw-rw-   0        0        0      296 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/sdkType.py
+-rw-rw-rw-   0        0        0     9064 2024-04-10 01:38:49.000000 azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/utils.py
+-rw-rw-rw-   0        0        0     5010 2024-04-10 01:38:49.000000 azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/web.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:39:43.365220 azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/
+-rw-rw-rw-   0        0        0     1497 2024-04-10 01:39:43.000000 azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2024-04-10 01:39:43.000000 azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:39:43.000000 azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-10 01:39:43.000000 azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 01:39:43.000000 azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1405 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:39:43.365220 azure-functions-extension-base-1.0.0a6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:39:43.355120 azure-functions-extension-base-1.0.0a6/tests/
+-rw-rw-rw-   0        0        0      519 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/tests/__init__.py
+-rw-rw-rw-   0        0        0    11526 2024-04-10 01:38:49.000000 azure-functions-extension-base-1.0.0a6/tests/test_meta.py
+-rw-rw-rw-   0        0        0      656 2024-04-10 01:38:45.000000 azure-functions-extension-base-1.0.0a6/tests/test_sdk_type.py
+-rw-rw-rw-   0        0        0    12756 2024-04-10 01:38:49.000000 azure-functions-extension-base-1.0.0a6/tests/test_utils.py
+-rw-rw-rw-   0        0        0    14668 2024-04-10 01:38:50.000000 azure-functions-extension-base-1.0.0a6/tests/test_web.py
```

### Comparing `azure-functions-extension-base-1.0.0a5/LICENSE` & `azure-functions-extension-base-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/PKG-INFO` & `azure-functions-extension-base-1.0.0a6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-functions-extension-base
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Base Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/__init__.py` & `azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     "HttpV2FeatureChecker",
     "ResponseLabels",
     "WebServer",
     "WebApp",
     "RequestSynchronizer",
 ]
 
-__version__ = "1.0.0a5"
+__version__ = "1.0.0a6"
```

### Comparing `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/meta.py` & `azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/meta.py`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/utils.py` & `azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/utils.py`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/web.py` & `azure-functions-extension-base-1.0.0a6/azure/functions/extension/base/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,29 +121,25 @@
             return cls._response_types is not None and any(
                 issubclass(pytype, response_type)
                 for response_type in cls._response_types.values()
             )
         return False
 
 
-class ABCModuleTrackerMeta(abc.ABCMeta, ModuleTrackerMeta):
-    pass
-
-
-class WebApp(metaclass=ABCModuleTrackerMeta):
+class WebApp(metaclass=ModuleTrackerMeta):
     @abstractmethod
     def route(self, func: Callable):
         raise NotImplementedError()
 
     @abstractmethod
     def get_app(self):
-        raise NotImplementedError()
+        raise NotImplementedError()  # pragma: no cover
 
 
-class WebServer(metaclass=ABCModuleTrackerMeta):
+class WebServer(metaclass=ModuleTrackerMeta):
     def __init__(self, hostname, port, web_app: WebApp):
         self.hostname = hostname
         self.port = port
         self.web_app = web_app.get_app()
 
     @abstractmethod
     async def serve(self):
```

### Comparing `azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/PKG-INFO` & `azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-functions-extension-base
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Base Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/SOURCES.txt` & `azure-functions-extension-base-1.0.0a6/azure_functions_extension_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/pyproject.toml` & `azure-functions-extension-base-1.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/tests/__init__.py` & `azure-functions-extension-base-1.0.0a6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/tests/test_meta.py` & `azure-functions-extension-base-1.0.0a6/tests/test_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         with self.assertRaises(ValueError):
             meta._BaseConverter._decode_typed_data(
                 datum_attempt_coerce, python_type=dict
             )
 
         # Case 7: attempt to coerce and pass
         datum_coerce_pass = meta.Datum(value=1, type="model_binding_data")
-        self.assertEquals(
+        self.assertEqual(
             meta._BaseConverter._decode_typed_data(datum_coerce_pass, python_type=str),
             "1",
         )
 
     def test_decode_trigger_metadata_field(self):
         datum_mbd = meta.Datum(value="{}", type="model_binding_data")
         mock_trigger_metadata = {"key": datum_mbd}
```

### Comparing `azure-functions-extension-base-1.0.0a5/tests/test_sdk_type.py` & `azure-functions-extension-base-1.0.0a6/tests/test_sdk_type.py`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/tests/test_utils.py` & `azure-functions-extension-base-1.0.0a6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a5/tests/test_web.py` & `azure-functions-extension-base-1.0.0a6/tests/test_web.py`

 * *Files 5% similar despite different names*

```diff
@@ -350,43 +350,25 @@
 
         mock_web_app = MockWebApp()
         server = MockWebServer("localhost", 8080, mock_web_app)
         self.assertEqual(server.hostname, "localhost")
         self.assertEqual(server.port, 8080)
         self.assertEqual(server.web_app, "MockApp")
 
-    async def test_serve_method_raises_not_implemented_error(self):
-        # Create a mock WebApp instance
-        class MockWebApp(WebApp):
-            def route(self, func):
-                pass
-
-            def get_app(self):
-                pass
-
-        class MockWebServer(WebServer):
-            async def serve(self):
-                super().serve()
-
-        # Create a WebServer instance with the mock WebApp
-        server = MockWebServer("localhost", 8080, MockWebApp())
-
-        # Ensure that calling the serve method raises NotImplementedError
-        with self.assertRaises(NotImplementedError):
-            await server.serve()
-
 
 class TestHttpV2Enabled(unittest.TestCase):
-    @patch("azure.functions.extension.base.ModuleTrackerMeta.module_imported")
-    def test_http_v2_enabled(self, mock_module_imported):
-        mock_module_imported.return_value = True
-        self.assertTrue(HttpV2FeatureChecker.http_v2_enabled())
+    def test_http_v2_enabled(self):
+        ModuleTrackerMeta._module = None
+
+        class MockClass(metaclass=ModuleTrackerMeta):
+            pass
 
-        mock_module_imported.return_value = False
-        self.assertFalse(HttpV2FeatureChecker.http_v2_enabled())
+        MockClass()
+
+        self.assertTrue(HttpV2FeatureChecker.http_v2_enabled())
 
 
 class TestResponseLabels(unittest.TestCase):
     def test_enum_values(self):
         self.assertEqual(ResponseLabels.STANDARD.value, "standard")
         self.assertEqual(ResponseLabels.STREAMING.value, "streaming")
         self.assertEqual(ResponseLabels.FILE.value, "file")
```

