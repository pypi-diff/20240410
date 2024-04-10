# Comparing `tmp/flask-variable-manager-0.2.0.tar.gz` & `tmp/flask-variable-manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-variable-manager-0.2.0.tar", last modified: Wed Apr  3 02:14:14 2024, max compression
+gzip compressed data, was "flask-variable-manager-0.3.0.tar", last modified: Wed Apr 10 08:25:30 2024, max compression
```

## Comparing `flask-variable-manager-0.2.0.tar` & `flask-variable-manager-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:14.921296 flask-variable-manager-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-03 02:14:14.917296 flask-variable-manager-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:14.917296 flask-variable-manager-0.2.0/flask_variable_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/flask_variable_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:14.917296 flask-variable-manager-0.2.0/flask_variable_manager/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/flask_variable_manager/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/flask_variable_manager/extension/variable_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:14.917296 flask-variable-manager-0.2.0/flask_variable_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/flask_variable_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/flask_variable_manager/tests/test_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:14.917296 flask-variable-manager-0.2.0/flask_variable_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-03 02:14:14.000000 flask-variable-manager-0.2.0/flask_variable_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 02:14:14.000000 flask-variable-manager-0.2.0/flask_variable_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:14:14.000000 flask-variable-manager-0.2.0/flask_variable_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 02:14:14.000000 flask-variable-manager-0.2.0/flask_variable_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 02:14:14.000000 flask-variable-manager-0.2.0/flask_variable_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 02:14:10.000000 flask-variable-manager-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:14:14.921296 flask-variable-manager-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/extension/variable_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/setup.cfg
```

### Comparing `flask-variable-manager-0.2.0/LICENSE` & `flask-variable-manager-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.2.0/PKG-INFO` & `flask-variable-manager-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,14 +86,28 @@
 
 This route allows you to remove a user-defined variable.
 
 It accepts a DELETE request at the `/vm/var` endpoint.
 
 (or `vm/vars` for the multiple count of the variable)
 
+### Run a Python script and return the result
+
+This route allows you to run a Python script and return the result.
+
+It accepts a POST request at the `/py/runner` endpoint.
+
+```python
+import platform
+from flask import g
+data = additionalProp + "-" + platform.platform()
+g.local['saved_user_variable'] = data
+return data
+```
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.2.0/README.md` & `flask-variable-manager-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -65,14 +65,28 @@
 
 This route allows you to remove a user-defined variable.
 
 It accepts a DELETE request at the `/vm/var` endpoint.
 
 (or `vm/vars` for the multiple count of the variable)
 
+### Run a Python script and return the result
+
+This route allows you to run a Python script and return the result.
+
+It accepts a POST request at the `/py/runner` endpoint.
+
+```python
+import platform
+from flask import g
+data = additionalProp + "-" + platform.platform()
+g.local['saved_user_variable'] = data
+return data
+```
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.2.0/flask_variable_manager/extension/variable_manager.py` & `flask-variable-manager-0.3.0/flask_variable_manager/extension/variable_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib
+from textwrap import indent
 
 from flask import g, jsonify, request, render_template_string
 
 
 def define_routes(app):
     @app.route('/vm/render', methods=['POST'])
     def render_template():
@@ -140,14 +141,50 @@
         """
         try:
             del g.local.to_dict()[key]
             return jsonify({'message': 'The variable has been cleared successfully.'})
         except KeyError:
             return jsonify({'message': 'The variable does not exist.'}), 404
 
+    @app.route('/py/runner', methods=['POST'])
+    def run_python_code():
+        """
+        ---
+        tags:
+          - Python
+        summary: Run Python code and return the result
+        description: This endpoint allows you to run Python code and return the result.
+        parameters:
+          - in: body
+            name: code
+            type: string
+            required: true
+            description: The Python code to run.
+        responses:
+          200:
+            description: The code has been executed successfully and the result is returned.
+            schema:
+              type: object
+              properties:
+                result:
+                  type: string
+                  description: The result of the executed code.
+        """
+        code = request.get_data(as_text=True)
+        wrapped_code = f"def _wrapped():\n{indent(code, '  ')}\nresult = _wrapped()"
+        local_vars = g.local.to_dict()
+        exec(wrapped_code, local_vars)
+        result = local_vars.get('result')
+        del local_vars["_wrapped"]
+        del local_vars["result"]
+        unwanted_keys = [key for key in local_vars if key.startswith('__') and key.endswith('__')]
+        for key in unwanted_keys:
+            del local_vars[key]
+        return jsonify({'result': str(result)})
+
 
 class VariableManagerExtension:
     def __init__(self, app=None):
         self._local = Local()
         if app is not None:
             self.init_app(app)
```

### Comparing `flask-variable-manager-0.2.0/flask_variable_manager/tests/test_vm.py` & `flask-variable-manager-0.3.0/flask_variable_manager/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.2.0/flask_variable_manager.egg-info/PKG-INFO` & `flask-variable-manager-0.3.0/flask_variable_manager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,14 +86,28 @@
 
 This route allows you to remove a user-defined variable.
 
 It accepts a DELETE request at the `/vm/var` endpoint.
 
 (or `vm/vars` for the multiple count of the variable)
 
+### Run a Python script and return the result
+
+This route allows you to run a Python script and return the result.
+
+It accepts a POST request at the `/py/runner` endpoint.
+
+```python
+import platform
+from flask import g
+data = additionalProp + "-" + platform.platform()
+g.local['saved_user_variable'] = data
+return data
+```
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.2.0/pyproject.toml` & `flask-variable-manager-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = ['flask_variable_manager*']
 
 [project]
 name = "flask-variable-manager"
-version = "0.2.0"
+version = "0.3.0"
 description = "Create a variable manager in flask, enter values in python, and use values on the jinja template."
 authors = [
     { name = "minwook-shin", email = "minwook0106@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

