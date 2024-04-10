# Comparing `tmp/openmeteo_sdk-1.8.0.tar.gz` & `tmp/openmeteo_sdk-1.9.0.tar.gz`

## Comparing `openmeteo_sdk-1.8.0.tar` & `openmeteo_sdk-1.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/Aggregation.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/Model.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/Unit.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/Variable.py
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/VariableWithValues.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/VariablesWithTime.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/WeatherApiResponse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/openmeteo_sdk/__init__.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/LICENSE
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/README.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    13540 2020-02-02 00:00:00.000000 openmeteo_sdk-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/Aggregation.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/Model.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/Unit.py
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/Variable.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/VariableWithValues.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/VariablesWithTime.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/WeatherApiResponse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/openmeteo_sdk/__init__.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/LICENSE
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/README.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13540 2020-02-02 00:00:00.000000 openmeteo_sdk-1.9.0/PKG-INFO
```

### Comparing `openmeteo_sdk-1.8.0/openmeteo_sdk/Model.py` & `openmeteo_sdk-1.9.0/openmeteo_sdk/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,7 +59,8 @@
     cma_grapes_global = 53
     bom_access_global = 54
     bom_access_global_ensemble = 55
     arpae_cosmo_seamless = 56
     arpae_cosmo_2i = 57
     arpae_cosmo_2i_ruc = 58
     arpae_cosmo_5m = 59
+    ecmwf_ifs025 = 60
```

### Comparing `openmeteo_sdk-1.8.0/openmeteo_sdk/Unit.py` & `openmeteo_sdk-1.9.0/openmeteo_sdk/Unit.py`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/openmeteo_sdk/Variable.py` & `openmeteo_sdk-1.9.0/openmeteo_sdk/Variable.py`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/openmeteo_sdk/VariableWithValues.py` & `openmeteo_sdk-1.9.0/openmeteo_sdk/VariableWithValues.py`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/openmeteo_sdk/VariablesWithTime.py` & `openmeteo_sdk-1.9.0/openmeteo_sdk/VariablesWithTime.py`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/openmeteo_sdk/WeatherApiResponse.py` & `openmeteo_sdk-1.9.0/openmeteo_sdk/WeatherApiResponse.py`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/.gitignore` & `openmeteo_sdk-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/LICENSE` & `openmeteo_sdk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/README.md` & `openmeteo_sdk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openmeteo_sdk-1.8.0/pyproject.toml` & `openmeteo_sdk-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name =  "openmeteo_sdk"
-version = "1.8.0"
+version = "1.9.0"
 authors = [
     {name = "Patrick Zippenfenig", email = "info@open-meteo.com"},
 ]
 description = "Open-Meteo Python SDK"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `openmeteo_sdk-1.8.0/PKG-INFO` & `openmeteo_sdk-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmeteo_sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Open-Meteo Python SDK
 Project-URL: Documentation, https://github.com/open-meteo/sdk/tree/main#readme
 Project-URL: Source, https://github.com/open-meteo/sdk
 Project-URL: Tracker, https://github.com/open-meteo/sdk/issues
 Author-email: Patrick Zippenfenig <info@open-meteo.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

