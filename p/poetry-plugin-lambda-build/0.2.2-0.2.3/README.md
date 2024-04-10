# Comparing `tmp/poetry_plugin_lambda_build-0.2.2.tar.gz` & `tmp/poetry_plugin_lambda_build-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_lambda_build-0.2.2.tar", max compression
+gzip compressed data, was "poetry_plugin_lambda_build-0.2.3.tar", max compression
```

## Comparing `poetry_plugin_lambda_build-0.2.2.tar` & `poetry_plugin_lambda_build-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-03-09 14:38:05.060870 poetry_plugin_lambda_build-0.2.2/LICENSE
--rw-r--r--   0        0        0     5653 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/__init__.py
--rw-r--r--   0        0        0     2176 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/docker.py
--rw-r--r--   0        0        0     6870 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/plugin.py
--rw-r--r--   0        0        0     6392 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/recipes.py
--rw-r--r--   0        0        0      543 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/utils.py
--rw-r--r--   0        0        0      652 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/zip.py
--rw-r--r--   0        0        0      706 2024-03-09 14:38:05.064870 poetry_plugin_lambda_build-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6314 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-10 13:55:11.583231 poetry_plugin_lambda_build-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5785 2024-04-10 13:55:11.583231 poetry_plugin_lambda_build-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 13:55:11.583231 poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/__init__.py
+-rw-r--r--   0        0        0     2176 2024-04-10 13:55:11.583231 poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/docker.py
+-rw-r--r--   0        0        0     7287 2024-04-10 13:55:11.583231 poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/plugin.py
+-rw-r--r--   0        0        0     6392 2024-04-10 13:55:11.583231 poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/recipes.py
+-rw-r--r--   0        0        0      543 2024-04-10 13:55:11.583231 poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/utils.py
+-rw-r--r--   0        0        0      652 2024-04-10 13:55:11.587231 poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/zip.py
+-rw-r--r--   0        0        0      706 2024-04-10 13:55:11.587231 poetry_plugin_lambda_build-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6446 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.2.3/PKG-INFO
```

### Comparing `poetry_plugin_lambda_build-0.2.2/LICENSE` & `poetry_plugin_lambda_build-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.2/README.md` & `poetry_plugin_lambda_build-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,15 @@
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
   docker_network_disabled    Disable networking ex. docker_network_disabled=0
   docker_network_mode        Network_mode
+  docker_platform            Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.
   package_install_dir        Installation directory inside zip artifact for single zip package
   layer_install_dir          Installation directory inside zip artifact for layer zip package
   function_install_dir       Installation directory inside zip artifact for function zip package
   package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
   function_artifact_path     Output function package path
   only                       The only dependency groups to include
```

### Comparing `poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/docker.py` & `poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/docker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/plugin.py` & `poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,25 +120,37 @@
         argument(*arg, optional=True, multiple=False) for arg in ARGS
     ]
 
     def _get_options(self) -> Any:
         options = defaultdict(dict)
         options.update(DEFAULT_OPTIONS)
         override_options = defaultdict(dict)
+        _missed_args = {}
 
         pyproject_data = self.poetry.pyproject.data
         # Gather override args
         for arg in ARGS:
             arg_name = arg[0]
-            _argument = self.argument(arg_name)
+            _argument = self.argument(arg_name) or _missed_args.get(arg_name)
             if _argument:
+                
+                if arg_name not in _argument:
+                    key = _argument.split("=", 1)[0]
+                    _missed_args[key] = _argument
+                    continue
+
                 try:
                     key, value = _argument.split("=", 1)
-                    prefix, name = key.split("_", 1)
-                    override_options[prefix][name] = value
+                    
+                    if "_" in key:
+                        prefix, name = key.split("_", 1)
+                        override_options[prefix][name] = value
+                    else:
+                        override_options[key] = value
+                    
                 except ValueError as e:
                     raise Exception(
                         f"Argument {arg_name} has wrong value: {_argument}", e
                     ) from e
 
         pyproject_data = self.poetry.pyproject.data
         prefixes = ["layer", "function", "docker", "artifacts"]
```

### Comparing `poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/recipes.py` & `poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/recipes.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/utils.py` & `poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.2/poetry_plugin_lambda_build/zip.py` & `poetry_plugin_lambda_build-0.2.3/poetry_plugin_lambda_build/zip.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.2/pyproject.toml` & `poetry_plugin_lambda_build-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-lambda-build"
-version = "0.2.2"
+version = "0.2.3"
 description = "The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more..."
 authors = ["Michał Murawski <mmurawski777@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^7.0.0"
```

### Comparing `poetry_plugin_lambda_build-0.2.2/PKG-INFO` & `poetry_plugin_lambda_build-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-lambda-build
-Version: 0.2.2
+Version: 0.2.3
 Summary: The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
 Author: Michał Murawski
 Author-email: mmurawski777@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -104,14 +104,15 @@
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
   docker_network_disabled    Disable networking ex. docker_network_disabled=0
   docker_network_mode        Network_mode
+  docker_platform            Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.
   package_install_dir        Installation directory inside zip artifact for single zip package
   layer_install_dir          Installation directory inside zip artifact for layer zip package
   function_install_dir       Installation directory inside zip artifact for function zip package
   package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
   function_artifact_path     Output function package path
   only                       The only dependency groups to include
```

