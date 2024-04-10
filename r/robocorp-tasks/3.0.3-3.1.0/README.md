# Comparing `tmp/robocorp_tasks-3.0.3.tar.gz` & `tmp/robocorp_tasks-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-3.0.3.tar", max compression
+gzip compressed data, was "robocorp_tasks-3.1.0.tar", max compression
```

## Comparing `robocorp_tasks-3.0.3.tar` & `robocorp_tasks-3.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rwxr-xr-x   0        0        0     2189 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/README.md
--rw-r--r--   0        0        0     1565 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     4325 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     7959 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1494 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     8261 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    28952 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      331 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_constants.py
--rw-r--r--   0        0        0        0 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/__init__.py
--rw-r--r--   0        0        0      572 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/_extension_points.py
--rw-r--r--   0        0        0     9934 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      242 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     5399 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_fixtures.py
--rw-r--r--   0        0        0     2396 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     7491 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     1022 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2881 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     4362 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0    13594 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_remove_refs.py
--rw-r--r--   0        0        0    10927 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     3837 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     3163 1970-01-01 00:00:00.000000 robocorp_tasks-3.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     2189 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/README.md
+-rw-r--r--   0        0        0     1565 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4325 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     7959 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1494 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     8261 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    30717 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      331 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_constants.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_customization/__init__.py
+-rw-r--r--   0        0        0     2136 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9934 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      242 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     5399 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_fixtures.py
+-rw-r--r--   0        0        0     2396 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     1022 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2881 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     5836 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0    13594 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_remove_refs.py
+-rw-r--r--   0        0        0    11485 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     3837 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:47:50.319345 robocorp_tasks-3.1.0/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     3163 1970-01-01 00:00:00.000000 robocorp_tasks-3.1.0/PKG-INFO
```

### Comparing `robocorp_tasks-3.0.3/README.md` & `robocorp_tasks-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/pyproject.toml` & `robocorp_tasks-3.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "3.0.3"
+version = "3.1.0"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
```

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/__init__.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from functools import wraps
 from pathlib import Path
 from typing import Dict, Optional
 
 from ._fixtures import setup, teardown
 from ._protocols import ITask, Status
 
-__version__ = "3.0.3"
+__version__ = "3.1.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(*args, **kwargs):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_callback.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_commands.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import json
 import os
 import sys
 import time
 import traceback
 import typing
 from argparse import ArgumentParser, ArgumentTypeError
+from ast import FunctionDef
 from io import StringIO
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Optional, Sequence, Union
+from typing import Any, Dict, List, Literal, Optional, Sequence, Union, overload
 
 from robocorp.tasks._customization._extension_points import EPManagedParameters
 from robocorp.tasks._protocols import ITask
 
 from . import _constants
 from ._argdispatch import arg_dispatch as _arg_dispatch
 from ._constants import SUPPORTED_TYPES_IN_SCHEMA
@@ -44,14 +45,15 @@
 
     Args:
         path: The path (file or directory) from where tasks should be collected.
     """
     from contextlib import redirect_stdout
 
     from robocorp.tasks._collect_tasks import collect_tasks
+    from robocorp.tasks._protocols import TasksListTaskTypedDict
     from robocorp.tasks._task import Context
 
     p = Path(path)
     context = Context()
     if not p.exists():
         context.show_error(f"Path: {path} does not exist")
         return 1
@@ -63,27 +65,27 @@
     if __stream__ is not None:
         write_to = __stream__
     else:
         write_to = original_stdout
 
     with redirect_stdout(sys.stderr):
         task: ITask
-        tasks_found = []
+        tasks_found: List[TasksListTaskTypedDict] = []
         for task in collect_tasks(pm, p, glob=glob):
-            tasks_found.append(
-                {
-                    "name": task.name,
-                    "line": task.lineno,
-                    "file": task.filename,
-                    "docs": getattr(task.method, "__doc__") or "",
-                    "input_schema": task.input_schema,
-                    "output_schema": task.output_schema,
-                    "options": task.options,
-                }
-            )
+            entry: TasksListTaskTypedDict = {
+                "name": task.name,
+                "line": task.lineno,
+                "file": task.filename,
+                "docs": getattr(task.method, "__doc__") or "",
+                "input_schema": task.input_schema,
+                "output_schema": task.output_schema,
+                "managed_params_schema": task.managed_params_schema,
+                "options": task.options,
+            }
+            tasks_found.append(entry)
 
         write_to.write(json.dumps(tasks_found))
         write_to.flush()
     return 0
 
 
 def _os_exit(retcode: int):
@@ -584,19 +586,19 @@
     type_hints = get_type_hints(target_method)
     method_name = target_method.__code__.co_name
     new_kwargs: Dict[str, Any] = {}
 
     for param_name, param in sig.parameters.items():
         param_type = type_hints.get(param_name)
 
-        is_managed_param = _is_managed_param(pm, param.name)
+        is_managed_param = _is_managed_param(pm, param.name, param=param)
         if param_type is None:
             # If not given, default to `str`.
             if is_managed_param:
-                param_type = _get_managed_param_type(pm, param.name)
+                param_type = _get_managed_param_type(pm, param)
             else:
                 param_type = str
 
         if param.default is inspect.Parameter.empty:
             # It's required, so, let's see if it's in the kwargs.
             if not is_managed_param:
                 if param_name not in kwargs:
@@ -631,46 +633,105 @@
             if not isinstance(passed_value, check_type):
                 raise InvalidArgumentsError(
                     f"Error. Expected the parameter: `{param_name}` to be of type: {param_type.__name__}. Found type: {type(passed_value).__name__}."
                 )
 
             new_kwargs[param_name] = passed_value
 
-    new_kwargs = _inject_managed_params(pm, sig, new_kwargs)
+    new_kwargs = _inject_managed_params(pm, sig, new_kwargs, kwargs)
     error_message = ""
     try:
         sig.bind(**new_kwargs)
     except Exception as e:
         error_message = f"It's not possible to call: '{method_name}' because the passed arguments don't match the expected signature.\nError: {e}"
     if error_message:
         raise InvalidArgumentsError(error_message)
 
     return new_kwargs
 
 
 def _inject_managed_params(
-    pm: PluginManager, sig: inspect.Signature, kwargs: Dict[str, Any]
+    pm: PluginManager,
+    sig: inspect.Signature,
+    new_kwargs: Dict[str, Any],
+    original_kwargs: Dict[str, Any],
 ) -> Dict[str, Any]:
     if pm.has_instance(EPManagedParameters):
         ep_managed_parameters = pm.get_instance(EPManagedParameters)
-        return ep_managed_parameters.inject_managed_params(sig, kwargs)
-    return kwargs
+        return ep_managed_parameters.inject_managed_params(
+            sig, new_kwargs, original_kwargs
+        )
+    return new_kwargs
+
+
+@overload
+def _is_managed_param(
+    pm: PluginManager,
+    param_name: str,
+    *,
+    node: FunctionDef,
+) -> bool:
+    pass
+
+
+@overload
+def _is_managed_param(
+    pm: PluginManager,
+    param_name: str,
+    *,
+    param: inspect.Parameter,
+) -> bool:
+    pass
+
 
+def _is_managed_param(
+    pm: PluginManager,
+    param_name: str,
+    *,
+    node: Optional[FunctionDef] = None,
+    param: Optional[inspect.Parameter] = None,
+) -> bool:
+    """
+    Verified if the given parameter is a managed parameter.
+
+    Args:
+        pm: The plugin manager.
+        param_name: The name of the parameter to check.
+        node: The FunctionDef node (ast), should be passed when doing lint
+            analysis.
+        param: The actual introspected parameter of the function, should
+            be passed when actually calling the function.
+
+    Returns: True if the given parameter is managed and False otherwise.
+
+    Note: either node or param must be passed (but not both at the same time).
+    """
+    if node is None and param is None:
+        raise AssertionError("Either node or param must be passed.")
+
+    if node is not None and param is not None:
+        raise AssertionError(
+            "Either the node or param must be passed, but not both at the same time."
+        )
 
-def _is_managed_param(pm: PluginManager, param_name: str) -> bool:
     if pm.has_instance(EPManagedParameters):
         ep_managed_parameters = pm.get_instance(EPManagedParameters)
-        return ep_managed_parameters.is_managed_param(param_name)
+        if node is not None:
+            return ep_managed_parameters.is_managed_param(param_name, node=node)
+        elif param is not None:
+            return ep_managed_parameters.is_managed_param(param_name, param=param)
+        else:
+            raise AssertionError("Not expected to get here.")
     return False
 
 
-def _get_managed_param_type(pm: PluginManager, param_name: str) -> type:
+def _get_managed_param_type(pm: PluginManager, param: inspect.Parameter) -> type:
     if pm.has_instance(EPManagedParameters):
         ep_managed_parameters = pm.get_instance(EPManagedParameters)
-        managed_param_type = ep_managed_parameters.get_managed_param_type(param_name)
+        managed_param_type = ep_managed_parameters.get_managed_param_type(param)
         assert managed_param_type is not None
         return managed_param_type
     raise RuntimeError(
         "Error: Asked managed param type for a param which is not managed."
     )
 
 
@@ -691,15 +752,15 @@
         prog=f"python -m {_constants.MODULE_ENTRY_POINT} {method_name} --",
         description=f"{method_name} task.",
         add_help=False,
     )
 
     # Add arguments to the parser based on the function signature and type hints
     for param_name, param in sig.parameters.items():
-        if _is_managed_param(pm, param.name):
+        if _is_managed_param(pm, param.name, param=param):
             continue
 
         param_type = type_hints.get(param_name)
 
         if param_type:
             if param_type not in SUPPORTED_TYPES_IN_SCHEMA:
                 if hasattr(param_type, "model_validate"):
```

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_config.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/_plugin_manager.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_fixtures.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_fixtures.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_interrupts.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_interrupts.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_protocols.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Any,
     Callable,
     Dict,
     Iterator,
     Optional,
     Sequence,
     Set,
+    TypedDict,
     TypeVar,
     Union,
 )
 
 ExcInfo = tuple[type[BaseException], BaseException, TracebackType]
 OptExcInfo = Union[ExcInfo, tuple[None, None, None]]
 
@@ -23,21 +24,23 @@
 Y = TypeVar("Y", covariant=True)
 
 
 def check_implements(x: T) -> T:
     """
     Helper to check if a class implements some protocol.
 
-    :important: It must be the last method in a class due to
-                https://github.com/python/mypy/issues/9266
+    Important: It must be the last method in a class due to
+        https://github.com/python/mypy/issues/9266
 
-        Example:
+    Example:
 
+    ```
     def __typecheckself__(self) -> None:
         _: IExpectedProtocol = check_implements(self)
+    ```
 
     Mypy should complain if `self` is not implementing the IExpectedProtocol.
     """
     return x
 
 
 class Status(str, Enum):
@@ -61,30 +64,84 @@
     # the value returned by the task.
     result: Any
 
     options: Optional[Dict]
 
     @property
     def input_schema(self) -> Dict[str, Any]:
-        pass
+        """
+        The input schema from the function signature.
+
+        Example:
+
+        ```
+        {
+            "properties": {
+                "value": {
+                    "type": "integer",
+                    "description": "Some value.",
+                    "title": "Value",
+                    "default": 0
+                }
+            },
+            "type": "object"
+        }
+        ```
+        """
 
     @property
     def output_schema(self) -> Dict[str, Any]:
-        pass
+        """
+        The output schema based on the function signature.
+
+        Example:
+
+        ```
+        {
+            "type": "string",
+            "description": ""
+        }
+        ```
+        """
+
+    @property
+    def managed_params_schema(self) -> Dict[str, Any]:
+        """
+        The schema for the managed parameters.
+
+        Example:
+
+        ```
+        {
+            "my_password": {
+                "type": "Secret"
+            },
+            "request": {
+                "type": "Request"
+            }
+        }
+        ```
+        """
 
     @property
     def name(self) -> str:
-        pass
+        """
+        The name of the task.
+        """
 
     @property
     def lineno(self) -> int:
-        pass
+        """
+        The line where the task is declared.
+        """
 
     def run(self) -> Any:
-        pass
+        """
+        Runs the task and returns its result.
+        """
 
     @property
     def failed(self) -> bool:
         """
         Returns true if the task failed.
         (in which case usually exc_info is not None).
         """
@@ -190,7 +247,23 @@
         pass
 
     def register(self, callback: ITaskCallback) -> IAutoUnregisterContextManager:
         pass
 
     def unregister(self, callback: ITaskCallback) -> None:
         pass
+
+
+class TasksListTaskTypedDict(TypedDict):
+    """
+    When python -m robocorp.tasks list is run, the output is a
+    list[TasksListTaskTypedDict].
+    """
+
+    name: str
+    line: int
+    file: str
+    docs: str
+    input_schema: Dict[str, Any]
+    output_schema: Dict[str, Any]
+    managed_params_schema: Dict[str, Any]
+    options: Optional[Dict]
```

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_remove_refs.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/_task.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,28 @@
         }
 
         if param_name:
             properties["title"] = param_name.replace("_", " ").title()
         return properties
 
     @property
+    def managed_params_schema(self) -> dict[str, Any]:
+        from robocorp.tasks._commands import _get_managed_param_type, _is_managed_param
+
+        managed_params_schema: Dict[str, Any] = {}
+        sig = inspect.signature(self.method)
+        for param in sig.parameters.values():
+            if _is_managed_param(self._pm, param.name, param=param):
+                tp = _get_managed_param_type(self._pm, param).__name__
+
+                managed_params_schema[param.name] = {"type": tp}
+
+        return managed_params_schema
+
+    @property
     def input_schema(self) -> dict[str, Any]:
         import docstring_parser
 
         from robocorp.tasks._commands import _is_managed_param
 
         sig = inspect.signature(self.method)
         method_name = self.method.__code__.co_name
@@ -131,15 +145,15 @@
 
         schema = {
             "properties": properties,
             "type": "object",
         }
 
         for param in sig.parameters.values():
-            if _is_managed_param(self._pm, param.name):
+            if _is_managed_param(self._pm, param.name, param=param):
                 continue
             param_type = type_hints.get(param.name)
             description = param_name_to_description.get(param.name, "")
             param_properties = self._build_properties(
                 method_name, param.name, param_type, description, "parameter"
             )
             properties[param.name] = param_properties
```

### Comparing `robocorp_tasks-3.0.3/src/robocorp/tasks/cli.py` & `robocorp_tasks-3.1.0/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.3/PKG-INFO` & `robocorp_tasks-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 3.0.3
+Version: 3.1.0
 Summary: The automation framework for Python
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

