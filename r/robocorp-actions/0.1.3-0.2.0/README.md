# Comparing `tmp/robocorp_actions-0.1.3.tar.gz` & `tmp/robocorp_actions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_actions-0.1.3.tar", max compression
+gzip compressed data, was "robocorp_actions-0.2.0.tar", max compression
```

## Comparing `robocorp_actions-0.1.3.tar` & `robocorp_actions-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     2958 2024-04-09 13:08:32.806096 robocorp_actions-0.1.3/README.md
--rw-r--r--   0        0        0      965 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3596 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/__init__.py
--rw-r--r--   0        0        0       81 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/__main__.py
--rw-r--r--   0        0        0      140 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_action_options.py
--rw-r--r--   0        0        0     5199 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     4243 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_fixtures.py
--rw-r--r--   0        0        0    11967 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_lint_action.py
--rw-r--r--   0        0        0     1211 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_managed_parameters.py
--rw-r--r--   0        0        0      314 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_protocols.py
--rw-r--r--   0        0        0     2907 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/_request_impl.py
--rw-r--r--   0        0        0     2123 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/cli.py
--rw-r--r--   0        0        0        0 2024-04-09 13:08:32.810096 robocorp_actions-0.1.3/src/robocorp/actions/py.typed
--rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 robocorp_actions-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2958 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/README.md
+-rw-r--r--   0        0        0      991 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3638 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/__main__.py
+-rw-r--r--   0        0        0     6717 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_action_context.py
+-rw-r--r--   0        0        0      140 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_action_options.py
+-rw-r--r--   0        0        0     5199 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     4243 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_fixtures.py
+-rw-r--r--   0        0        0    11984 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_lint_action.py
+-rw-r--r--   0        0        0     4359 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_managed_parameters.py
+-rw-r--r--   0        0        0      561 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_protocols.py
+-rw-r--r--   0        0        0     2907 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_request_impl.py
+-rw-r--r--   0        0        0     4480 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_secret.py
+-rw-r--r--   0        0        0     2123 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/py.typed
+-rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 robocorp_actions-0.2.0/PKG-INFO
```

### Comparing `robocorp_actions-0.1.3/README.md` & `robocorp_actions-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.3/pyproject.toml` & `robocorp_actions-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "robocorp-actions"
-version = "0.1.3"
+version = "0.2.0"
 description = "Robocorp Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
 packages = [{ include = "robocorp", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 # robocorp-actions is tighly coupled with robocorp-tasks, so,
 # the version must be an exact match up to the minor version.
-robocorp-tasks = "3.0.3"
+robocorp-tasks = "3.1.1"
+cryptography = "^42.0.5"
+
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = { path = "../devutils/", develop = true }
 
 # We just need it for tests. In runtime duck-typing is used to
 # check for `cls.parse_obj(dict)` and `cls.model_json_schema()`
 pydantic = "^2.6"
```

### Comparing `robocorp_actions-0.1.3/src/robocorp/actions/__init__.py` & `robocorp_actions-0.2.0/src/robocorp/actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from pathlib import Path
 from typing import Callable, Optional, overload
 
 from ._action_options import ActionOptions
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
+from ._secret import Secret
 
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
 
@@ -122,14 +123,15 @@
 
     return get_current_task()
 
 
 __all__ = [
     "IAction",
     "Request",
+    "Secret",
     "Status",
     "action",
     "action_cache",
     "get_current_action",
     "get_output_dir",
     "session_cache",
     "setup",
```

### Comparing `robocorp_actions-0.1.3/src/robocorp/actions/_args_dispatcher.py` & `robocorp_actions-0.2.0/src/robocorp/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.3/src/robocorp/actions/_fixtures.py` & `robocorp_actions-0.2.0/src/robocorp/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.3/src/robocorp/actions/_lint_action.py` & `robocorp_actions-0.2.0/src/robocorp/actions/_lint_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             coldelta=4,
             severity=DiagnosticSeverity.Warning,
         )
 
     if arguments.args:
         for arg in arguments.args:
             desc = param_name_to_description.pop(arg.arg, None)
-            if pm is not None and _is_managed_param(pm, arg.arg):
+            if pm is not None and _is_managed_param(pm, arg.arg, node=node):
                 continue
 
             if not desc:
                 yield _make_error(
                     arg,
                     f"Parameter: `{arg.arg}` documentation not found in docstring. "
                     "Please update docstring to add it as an LLM needs this info "
@@ -281,15 +281,15 @@
                     f"Parameter: `{arg.arg}` without annotation "
                     "(considering `str` as the expected type).",
                     severity=DiagnosticSeverity.Warning,
                 )
 
 
 def iter_lint_errors(
-    action_contents_file: str | bytes, pm: Optional[PluginManager] = None
+    action_contents_file: Union[str, bytes], pm: Optional[PluginManager] = None
 ) -> Iterator[Error]:
     ast = ast_module.parse(action_contents_file, "<string>")
     for _stack, node in _iter_nodes(ast, recursive=False):
         if isinstance(node, ast_module.FunctionDef):
             for decorator in node.decorator_list:
                 if isinstance(decorator, ast_module.Name) and decorator.id == "action":
                     # We found an @action. Do the needed checks.
```

### Comparing `robocorp_actions-0.1.3/src/robocorp/actions/_request.py` & `robocorp_actions-0.2.0/src/robocorp/actions/_request.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.3/src/robocorp/actions/_request_impl.py` & `robocorp_actions-0.2.0/src/robocorp/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.3/src/robocorp/actions/cli.py` & `robocorp_actions-0.2.0/src/robocorp/actions/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.3/PKG-INFO` & `robocorp_actions-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp-actions
-Version: 0.1.3
+Version: 0.2.0
 Summary: Robocorp Actions
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: robocorp-tasks (==3.0.3)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
+Requires-Dist: robocorp-tasks (==3.1.1)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # ⚡️ robocorp-actions
 
 A Python library designed to simplify the development of Python actions _(AI or otherwise)_ to be run with the [Robocorp Action Server](../action_server/).
```

