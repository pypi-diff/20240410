# Comparing `tmp/toolfuse-0.1.13.tar.gz` & `tmp/toolfuse-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.13.tar", max compression
+gzip compressed data, was "toolfuse-0.1.15.tar", max compression
```

## Comparing `toolfuse-0.1.13.tar` & `toolfuse-0.1.15.tar`

### file list

```diff
@@ -1,24 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-04-08 12:48:37.563544 toolfuse-0.1.13/LICENSE
--rw-r--r--   0        0        0     3332 2024-04-08 12:48:37.563544 toolfuse-0.1.13/README.md
--rw-r--r--   0        0        0      783 2024-04-08 12:48:37.567544 toolfuse-0.1.13/pyproject.toml
--rw-r--r--   0        0        0      341 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/__init__.py
--rw-r--r--   0        0        0    19516 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/base.py
--rw-r--r--   0        0        0       72 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/__init__.py
--rw-r--r--   0        0        0     3144 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/exceptions.py
--rw-r--r--   0        0        0     8765 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/func.py
--rw-r--r--   0        0        0      161 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/json_type.py
--rw-r--r--   0        0        0      157 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/__init__.py
--rw-r--r--   0        0        0     1920 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/abc.py
--rw-r--r--   0        0        0     1011 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      202 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/bool_parser.py
--rw-r--r--   0        0        0     2410 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      761 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/default.py
--rw-r--r--   0        0        0     1325 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/dict_parser.py
--rw-r--r--   0        0        0     1442 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/enum_parser.py
--rw-r--r--   0        0        0      569 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/float_parser.py
--rw-r--r--   0        0        0      691 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/int_parser.py
--rw-r--r--   0        0        0     1043 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/list_parser.py
--rw-r--r--   0        0        0      735 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/none_parser.py
--rw-r--r--   0        0        0      205 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/str_parser.py
--rw-r--r--   0        0        0     1304 2024-04-08 12:48:37.567544 toolfuse-0.1.13/toolfuse/function/parsers/union_parser.py
--rw-r--r--   0        0        0     3987 1970-01-01 00:00:00.000000 toolfuse-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.15/LICENSE
+-rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.15/README.md
+-rw-r--r--   0        0        0      803 2024-04-10 15:05:04.066332 toolfuse-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.15/toolfuse/__init__.py
+-rw-r--r--   0        0        0    19587 2024-04-10 15:04:52.103260 toolfuse-0.1.15/toolfuse/base.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.15/PKG-INFO
```

### Comparing `toolfuse-0.1.13/LICENSE` & `toolfuse-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.13/README.md` & `toolfuse-0.1.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     <a href="https://github.com/agentsea/toolfuse/issues">Report Bug</a>
     ·
     <a href="https://github.com/agentsea/toolfuse/issues">Request Feature</a>
   </p>
   <br>
 </p>
 
-ToolFuse provides a common potocol for AI agent tools, use them with your favorite agent framework or model.
+ToolFuse provides a common protocol for AI agent tools, use them with your favorite agent framework or model.
 
 ## Installation
 
 ```
 pip install toolfuse
 ```
```

### Comparing `toolfuse-0.1.13/pyproject.toml` & `toolfuse-0.1.15/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.13"
+version = "0.1.15"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 docstring-parser = "^0.15"
 urllib3 = "^1.26.0"
 python-dotenv = "^1.0.1"
 openai = "^1.12.0"
+toolcore = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 recommonmark = "^0.7.1"
 flake8 = "^7.0.0"
 black = "^24.2.0"
```

### Comparing `toolfuse-0.1.13/toolfuse/base.py` & `toolfuse-0.1.15/toolfuse/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 from typing import List, Callable, Any, Dict, Optional, TypeVar, Type, Union
 from inspect import getdoc
 import inspect
 import re
 
-from .function import FunctionWrapper
+from toolcore import FunctionWrapper
 
 
 class Action:
     """
     Represents an action that an agent can perform in an environment.
 
     This class is used to encapsulate information about an action, including its
@@ -127,15 +127,15 @@
 
     Args:
         method (Callable): The method to be marked as an action.
 
     Returns:
         Callable: The original method with the added '_is_action' attribute.
     """
-    method._is_action = True
+    method._is_action = True  # type: ignore
     return method
 
 
 def observation(method: Callable) -> Callable:
     """
     A decorator that marks a method as an observation within the Tool.
 
@@ -146,15 +146,15 @@
 
     Args:
         method (Callable): The method to be marked as an observation.
 
     Returns:
         Callable: The original method with the added '_is_observation' attribute.
     """
-    method._is_observation = True
+    method._is_observation = True  # type: ignore
     return method
 
 
 T = TypeVar("T")
 
 
 class Tool(ABC):
@@ -320,23 +320,24 @@
 
     def context(self) -> str:
         """LLM context fork the tool
 
         Returns:
             str: LLM context for the tool
         """
-        return self.__doc__
+        return self.__doc__  # type: ignore
 
-    def name(self) -> str:
+    @classmethod
+    def name(cls) -> str:
         """Tool name
 
         Returns:
             str: Tool name
         """
-        return self.__class__.__name__
+        return cls.__name__
 
 
 def tool_from_cls(cls: Type[T]) -> Type[Tool]:
     """
     Dynamically creates a subclass of `Tool` that integrates methods from a given class `cls` as actions.
 
     Args:
@@ -344,19 +345,20 @@
 
     Returns:
         Type[Tool]: A new subclass of Tool that includes actions derived from `cls` methods.
     """
 
     class Combined(Tool, cls):
         def __init__(self, *args, **kwargs):
-            cls.__init__(self, *args, **kwargs)  # Initialize the original class
+            cls.__init__(self, *args, **kwargs)  # type: ignore
             Tool.__init__(self)  # Initialize the Tool part of the combined class
             self._register_methods_from_cls()
 
-        def name(self) -> str:
+        @classmethod
+        def name(cls) -> str:
             return cls.__name__
 
         def _register_methods_from_cls(self):
             """
             Registers all public methods of `cls` as actions for the Tool.
             """
             for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
@@ -479,15 +481,15 @@
                 action = Action(name, method, schema, description)
 
                 # Add the Action to the tool's actions list
                 self._actions_list.append(action)
 
     ObjectTool.__name__ = f"{obj.__class__.__name__}Tool"
     # Return an instance of ObjectTool instead of the class itself, as we need to pass the object instance to it
-    return ObjectTool(obj)
+    return ObjectTool(obj)  # type: ignore
 
 
 def tool(input: Union[Type, Callable, Any]) -> Union[Type[Tool], Tool]:
     """
     Dynamically creates a Tool instance or class based on the type of the input.
 
     This function determines whether the input is a class, a function, or an object instance
```

### Comparing `toolfuse-0.1.13/PKG-INFO` & `toolfuse-0.1.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.13
+Version: 0.1.15
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: toolcore (>=0.1.0,<0.2.0)
 Requires-Dist: urllib3 (>=1.26.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <!-- <a href="https://github.com/agentsea/skillpacks">
@@ -37,15 +37,15 @@
     <a href="https://github.com/agentsea/toolfuse/issues">Report Bug</a>
     ·
     <a href="https://github.com/agentsea/toolfuse/issues">Request Feature</a>
   </p>
   <br>
 </p>
 
-ToolFuse provides a common potocol for AI agent tools, use them with your favorite agent framework or model.
+ToolFuse provides a common protocol for AI agent tools, use them with your favorite agent framework or model.
 
 ## Installation
 
 ```
 pip install toolfuse
 ```
```

