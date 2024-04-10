# Comparing `tmp/revel-0.8.9.tar.gz` & `tmp/revel-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revel-0.8.9.tar", max compression
+gzip compressed data, was "revel-0.9.0.tar", max compression
```

## Comparing `revel-0.8.9.tar` & `revel-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2332 2023-11-08 19:51:02.358299 revel-0.8.9/README.md
--rw-r--r--   0        0        0      620 2023-12-12 17:58:29.905009 revel-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      353 2023-12-08 21:18:24.218135 revel-0.8.9/revel/__init__.py
--rw-r--r--   0        0        0    19959 2023-12-12 17:01:59.779983 revel-0.8.9/revel/argument_parser.py
--rw-r--r--   0        0        0    11705 2023-12-08 21:18:24.228135 revel-0.8.9/revel/cli_app.py
--rw-r--r--   0        0        0     4468 2023-11-08 19:51:04.001634 revel-0.8.9/revel/common.py
--rw-r--r--   0        0        0     1692 2023-11-08 19:51:03.998300 revel-0.8.9/revel/errors.py
--rw-r--r--   0        0        0    31438 2023-12-08 21:18:24.221468 revel-0.8.9/revel/legacy.py
--rw-r--r--   0        0        0      723 2023-11-08 19:51:03.998300 revel-0.8.9/revel/markup.py
--rw-r--r--   0        0        0     7412 2023-11-08 19:51:03.998300 revel-0.8.9/revel/menu.py
--rw-r--r--   0        0        0       80 2023-11-08 19:51:04.001634 revel-0.8.9/revel/rapidbaby/__init__.py
--rw-r--r--   0        0        0      274 2023-11-08 19:51:04.001634 revel-0.8.9/revel/rapidbaby/common.py
--rw-r--r--   0        0        0     7117 2023-11-08 19:51:04.001634 revel-0.8.9/revel/rapidbaby/parser.py
--rw-r--r--   0        0        0     5803 2023-11-08 19:51:04.001634 revel-0.8.9/revel/rapidbaby/styles.py
--rw-r--r--   0        0        0     2109 2023-12-08 21:18:24.221468 revel-0.8.9/revel/shell_escape.py
--rw-r--r--   0        0        0      815 2023-11-08 19:51:04.001634 revel-0.8.9/revel/style.py
--rw-r--r--   0        0        0     2973 1970-01-01 00:00:00.000000 revel-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     2332 2023-11-08 19:51:02.358299 revel-0.9.0/README.md
+-rw-r--r--   0        0        0      698 2024-04-10 20:53:17.464413 revel-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-10 19:36:28.949450 revel-0.9.0/revel/__init__.py
+-rw-r--r--   0        0        0    19979 2024-04-10 20:42:29.987625 revel-0.9.0/revel/argument_parser.py
+-rw-r--r--   0        0        0    12853 2024-04-10 20:49:41.346830 revel-0.9.0/revel/cli_app.py
+-rw-r--r--   0        0        0     4912 2024-04-10 19:35:14.694203 revel-0.9.0/revel/common.py
+-rw-r--r--   0        0        0     1919 2024-04-10 19:36:28.959449 revel-0.9.0/revel/errors.py
+-rw-r--r--   0        0        0    32100 2024-04-10 19:40:05.148617 revel-0.9.0/revel/legacy.py
+-rw-r--r--   0        0        0      723 2023-11-08 19:51:03.998300 revel-0.9.0/revel/markup.py
+-rw-r--r--   0        0        0     7533 2024-04-10 19:40:50.824400 revel-0.9.0/revel/menu.py
+-rw-r--r--   0        0        0       80 2023-11-08 19:51:04.001634 revel-0.9.0/revel/rapidbaby/__init__.py
+-rw-r--r--   0        0        0      274 2023-11-08 19:51:04.001634 revel-0.9.0/revel/rapidbaby/common.py
+-rw-r--r--   0        0        0     7136 2024-02-04 09:24:39.690123 revel-0.9.0/revel/rapidbaby/parser.py
+-rw-r--r--   0        0        0     5836 2024-02-04 09:24:50.466800 revel-0.9.0/revel/rapidbaby/styles.py
+-rw-r--r--   0        0        0     2106 2024-02-04 09:24:16.310104 revel-0.9.0/revel/shell_escape.py
+-rw-r--r--   0        0        0      815 2023-11-08 19:51:04.001634 revel-0.9.0/revel/style.py
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 revel-0.9.0/PKG-INFO
```

### Comparing `revel-0.8.9/README.md` & `revel-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `revel-0.8.9/pyproject.toml` & `revel-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "revel"
-version = "0.8.9"
+version = "0.9.0"
 description = "Effortlessly spice up your terminal apps using colors, progressbars & more"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
+repository = "https://gitlab.com/Vivern/revel"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 blessed = "^1.19.1"
 readchar = "^4.0.3"
 colorama = "^0.4.6"
+typing-extensions = "^4.10.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 black = "^22.10.0"
 isort = "^5.10.1"
 pre-commit = "^2.20.0"
 ipykernel = "^6.22.0"
```

### Comparing `revel-0.8.9/revel/argument_parser.py` & `revel-0.9.0/revel/argument_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import re
+import types
 from dataclasses import dataclass
 from typing import *  # type: ignore
 from typing import Any
 
 import revel
 
 from . import common, legacy, menu
@@ -27,38 +28,38 @@
 
 @dataclass
 class Parameter:
     # Name, as presented to the user
     name: str
 
     # Optionally a single-character shorthand for the parameter
-    shorthand: Optional[str]
+    shorthand: str | None
 
     # How the parameter is called in python. This is needed when passing it to
     # a function as a keyword argument.
     python_name: str
 
     # If asking interactively for this parameter, this text will be used as the
     # prompt. Falls back to the name if not specified.
-    prompt: Optional[str]
+    prompt: str | None
 
     type: Type
 
     is_flag: bool
     is_variadic: bool
 
     default_value: Any
 
     def __hash__(self) -> int:
         return hash(id(self))
 
 
 def parameters_from_function(
     function: Callable,
-) -> Iterable[Tuple[inspect.Parameter, Parameter]]:
+) -> Iterable[tuple[inspect.Parameter, Parameter]]:
     """
     Converts the given function's parameter list into a list of `Parameter`s.
     """
     signature = inspect.signature(function)
     type_hints = get_type_hints(function)
 
     for name, parameter in signature.parameters.items():
@@ -116,46 +117,39 @@
             is_flag=is_flag,
             is_variadic=is_variadic,
             default_value=default_value,
         )
 
 
 def _parse_literal(raw: str, typ: Type) -> str:
-    # TODO: Normalize?
-    # Assign scores for each match?
+    options = get_args(typ)
 
-    # Find all matches
-    possible_values = get_args(typ)
-    matches = []
-
-    for possible_value in possible_values:
-        # Exact match? This is it
-        if raw == possible_value:
-            return possible_value
-
-        # Partial match? Keep it
-        if raw in possible_value:
-            matches.append(possible_value)
-
-    # No matches? Error
-    if not matches:
-        possible_values_str = common.comma_separated_list(possible_values, "and", "`")
+    # Figure out which option the user is referring to
+    try:
+        selected_index = common.choose_string(
+            options=[[value] for value in options],
+            selection=raw,
+        )
+
+    # No match?
+    except NoSuchOptionError:
+        options_str = common.comma_separated_list(options, "and", "`")
         raise ArgumentError(
-            f"`{raw}` is not a valid value for `{typ}`. Pass one of {possible_values_str}"
+            f"`{raw}` is not valid here. Please provide one of {options_str}"
         )
 
     # Multiple matches? Ambiguous
-    if len(matches) > 1:
-        matches_str = common.comma_separated_list(matches, "or", "`")
+    except AmbiguousOptionError as err:
+        options_str = common.comma_separated_list(err.matching_options, "and", "`")
         raise ArgumentError(
-            f"`{raw}` is ambiguous for `{typ}`. It could refer to either of {matches_str}"
+            f"`{raw}` is ambiguous here. It could refer to either of {options_str}"
         )
 
-    # Exactly one match? This is it
-    return matches[0]
+    # There was a match. Return it
+    return options[selected_index]
 
 
 def _parse_bool(raw: str) -> bool:
     raw = raw.lower()
 
     if raw in ("true", "t", "yes", "y", "1"):
         return True
@@ -181,14 +175,17 @@
 
 
 def parse_value(value: str, typ: Type) -> Any:
     type_key = get_origin(typ)
     if type_key is None:
         type_key = typ
 
+    if hasattr(types, "UnionType") and type_key is types.UnionType:
+        type_key = Union
+
     if type_key in (str, Any):
         return str(value)
 
     if type_key is Literal:
         return _parse_literal(value, typ)
 
     if type_key is bool:
@@ -217,51 +214,51 @@
 
 
 class Parser:
     def __init__(self, parameters: Iterable[Parameter]):
         self.parameters = list(parameters)
 
         # All parameters, by their name, shorthand, and position
-        self.parameters_by_name: Dict[str, Parameter] = {}
-        self.parameters_by_shorthand: Dict[str, Parameter] = {}
-        self.positional_parameters: List[Parameter] = []
+        self.parameters_by_name: dict[str, Parameter] = {}
+        self.parameters_by_shorthand: dict[str, Parameter] = {}
+        self.positional_parameters: list[Parameter] = []
 
         for parameter in self.parameters:
             # Positional or flag?
             if parameter.is_flag:
                 self.parameters_by_name[parameter.name] = parameter
 
                 if parameter.shorthand is not None:
                     self.parameters_by_shorthand[parameter.shorthand] = parameter
             else:
                 self.positional_parameters.append(parameter)
 
         # Maps already assigned values to parameters
-        self.assigned_parameters: Dict[str, List[str]] = {}
+        self.assigned_parameters: dict[str, list[str]] = {}
 
         # If not `None`, this is the parameter that is currently looking for a
         # value
-        self.current_parameter: Optional[str] = None
+        self.current_parameter: str | None = None
 
         # Whether any more flags are allowed
         self.allow_flags = True
 
         # Any superfluous values which cannot be assigned to any parameter
-        self.rest: List[str] = []
+        self.rest: list[str] = []
 
         # Any errors that occurred during parsing
-        self.errors: List[str] = []
+        self.errors: list[str] = []
 
         # The index of the next positional parameter to assign a value to
         self.next_positional_parameter_index = 0
 
     def _feed_flags(
         self,
         flag_names: Iterable[str],
-        flag_value: Optional[str],
+        flag_value: str | None,
         use_shorthands: bool,
     ) -> None:
         flag_names = list(flag_names)
         flag_by_name_dict = (
             self.parameters_by_shorthand if use_shorthands else self.parameters_by_name
         )
 
@@ -372,15 +369,15 @@
         for value in values:
             self.feed_one(value)
 
     def finish(
         self,
         *,
         allow_missing_arguments: bool = False,
-    ) -> Dict[Parameter, Any]:
+    ) -> dict[Parameter, Any]:
         """
         Complete the parsing process and return the assigned values.
         """
 
         # Make sure no parameter is still looking for a value
         if self.current_parameter is not None:
             self.errors.append(f"Missing value for `{self.current_parameter}`")
@@ -438,15 +435,15 @@
         # Done
         return result
 
 
 def ask_value_for_parameter(
     param: Parameter,
     *,
-    prompt: Optional[str] = None,
+    prompt: str | None = None,
 ) -> Any:
     """
     Ask the user for a value for the given parameter, parse and return it.
     """
     if prompt is None:
         prompt = " ".join(param.name.split("-")).title()
 
@@ -486,19 +483,19 @@
         try:
             return parse_value(value, param.type)
         except ArgumentError as e:
             revel.error(e.message)
 
 
 def parse_function_parameters(
-    params: List[Parameter],
+    params: list[Parameter],
     raw_args: Iterable[str],
     *,
     interactive: bool = False,
-) -> Tuple[List[Any], Dict[str, Any]]:
+) -> tuple[list[Any], dict[str, Any]]:
     """
     Given a list of parameters, parse the given arguments and return them in a
     form usable to call the function. If `interactive` is `True`, ask for any
     missing values interactively.
 
     The result is a tuple of args and kwargs, which can be used to call the
     target function as `target(*args, **kwargs)`.
@@ -556,21 +553,22 @@
             by_position.append(value)
 
     # Done
     return by_position, by_name
 
 
 def parse_function_name(
-    function_names: List[str],
-    function_summaries: List[Optional[str]],
-    raw_args: List[str],
+    function_names: list[str],
+    function_summaries: list[str | None],
+    raw_args: list[str],
     *,
-    function_aliases: Optional[List[Set[str]]] = None,
+    function_aliases: list[Set[str]] | None = None,
     interactive: bool = False,
-) -> Tuple[str, List[str]]:
+    option_name: str = "function",
+) -> tuple[str, list[str]]:
     """
     Given a list of functions and their names, extract the name of the function
     to call from the given arguments. The function name is expected to be the
     first argument, and the remainder are returned.
 
     If no function name was provided, and `interactive` is `True`, ask for the
     function name interactively.
@@ -586,50 +584,50 @@
             `interactive` is `False`.
     """
     if function_aliases is None:
         function_aliases = [set() for _ in function_names]
 
     # See if the user has specified a function name
     if raw_args:
-        all_names_and_aliases: List[List[str]] = []
+        all_names_and_aliases: list[list[str]] = []
 
         for name, aliases in zip(function_names, function_aliases):
             all_names_and_aliases.append([name] + list(aliases))
 
         try:
             choice_index = common.choose_string(
-                choices=all_names_and_aliases,
+                options=all_names_and_aliases,
                 selection=raw_args[0],
             )
 
         except NoSuchOptionError as e:
             # Can't ask, raise an exception
             if not interactive:
                 raise e
 
-            legacy.warning(e.message)
+            legacy.warning(e.message(option_name=option_name))
             print()
 
         except AmbiguousOptionError as e:
             # Can't ask, raise an exception
             if not interactive:
                 raise e
 
-            legacy.warning(e.message)
+            legacy.warning(e.message(option_name=option_name))
             print()
 
         else:
             # If the command was referenced via an alias, point the user to the
             # canonical name
             entered_name = raw_args[0]
             proper_name = function_names[choice_index]
 
             if entered_name != proper_name:
                 legacy.warning(
-                    f"There is no command named [primary]{entered_name}[/]. Assuming you meant to type [primary]{proper_name}[/]."
+                    f"There is no {option_name} named [primary]{entered_name}[/]. Assuming you meant to type [primary]{proper_name}[/]."
                 )
                 print()
 
             return function_names[choice_index], raw_args[1:]
 
     # Nothing specified, and can't ask -> raise an exception
     if not interactive:
```

### Comparing `revel-0.8.9/revel/cli_app.py` & `revel-0.9.0/revel/cli_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,138 @@
 import sys
 from dataclasses import KW_ONLY, dataclass
 from typing import *  # type: ignore
 
+import typing_extensions
+
 from . import argument_parser, common
 from .errors import (
     AmbiguousOptionError,
     ArgumentError,
     NoOptionGivenError,
     NoSuchOptionError,
 )
 from .legacy import error, print, warning
 
+P = typing_extensions.ParamSpec("P")
+R = TypeVar("R")
+
 
 @dataclass(frozen=True)
 class Parameter:
     name: str
     _ = KW_ONLY
-    summary: Optional[str] = None
-    prompt: Optional[str] = None
+    summary: str | None = None
+    prompt: str | None = None
 
 
 @dataclass(frozen=True)
 class AppCommand:
     # The name to use for this command
     name: str
 
     # Additional names that can be used to invoke this command
     aliases: Set[str]
 
     # Short description of the command
-    summary: Optional[str]
+    summary: str | None
 
     # Longer, detailed description of the command
-    details: Optional[str]
+    details: str | None
 
     # Any parameters the user has provided to describe this command. These may
     # be fewer than the function's parameters, or empty altogether.
-    user_provided_parameters: List[Parameter]
+    user_provided_parameters: list[Parameter]
 
     # The function to call when this command is invoked
     function: Callable
 
 
 class App:
     def __init__(
         self,
         *,
-        name: Optional[str] = None,
-        summary: Optional[str] = None,
-        details: Optional[str] = None,
+        nicename: str,
+        command_name: str,
+        summary: str | None = None,
+        details: str | None = None,
+        version: str | None = None,
         add_help_command: bool = True,
-        add_version_command: bool = True,
-    ):
-        if name is None:
-            self.name = "TODO-auto-detect-app-name"
-        else:
-            self.name = name.strip()
+    ) -> None:
+        """
+        Creates a new CLI app. The app contains all information to run a CLI
+        application, including commands, options, and help text.
+
+        ## Args
+
+        `nicename`: A human-readable, nice name for the application. This will
+        be used in texts to refer to the application.
+
+        `command_name`: The name of the command that will be used to run the app
+        from the terminal.
 
+        `summary`: A short description of the application. Should be at most one
+        line.
+
+        `details`: A longer, more detailed description of the application. This
+        may span multiple paragraphs and will only be displayed when the user
+        asks for it, such as in the help text.
+
+        `version`: The version of the application. If provided, a `version`
+        command will be added.
+
+        `add_help_command`: If `True`, a `help` command will be added to the
+        app.
+        """
+
+        self.nicename = nicename
+        self.command_name = command_name
         self.summary = None if summary is None else summary.strip()
         self.details = None if details is None else common.multiline_strip(details)
-        self._commands: List[AppCommand] = []
+        self.version = version
+        self._commands: list[AppCommand] = []
 
-        # Add built-in commands
+        # Add the `help` command
         if add_help_command:
             self.command(
                 name="help",
                 summary="Display help for a command",
-                details="""
-If not command is provided, this command will show general help for the
-application. If a command is provided, shows help for that command instead.
+                details=f"""
+If no command is provided, this will show general help for {self.nicename}. If a command
+is provided, shows help for that command instead.
                 """,
             )(self._display_help)
 
-        if add_version_command:
+        # Add the `version` command
+        if version is not None:
             self.command(
                 name="version",
-                summary=f"Display version information for {self.name}",
+                summary=f"Display version information for {self.nicename}",
             )(self._display_version)
 
-    def _display_help(self, command: Optional[str] = None) -> None:
+    def _display_help(self, command: str | None = None) -> None:
         # Was a valid command specified?
-        cmd_instance: Optional[AppCommand] = None
+        cmd_instance: AppCommand | None = None
 
         if command is not None:
             try:
-                all_names_and_aliases: List[List[str]] = []
+                all_names_and_aliases: list[list[str]] = []
 
                 for cmd in self._commands:
                     all_names_and_aliases.append([cmd.name] + list(cmd.aliases))
 
                 cmd_index = common.choose_string(
                     all_names_and_aliases,
                     command,
                 )
             except NoSuchOptionError as err:
-                error(f"There is no command named `{err.entered_command}`")
+                error(err.message(option_name="command"))
                 print()
             except AmbiguousOptionError as err:
-                error(err.message)
+                error(err.message(option_name="command"))
                 print()
             else:
                 cmd_instance = self._commands[cmd_index]
 
         # If not command was provided, or the given one doesn't exist, display
         # general help
         if cmd_instance is None:
@@ -214,28 +245,24 @@
 
         # Details
         if cmd_instance.details is not None:
             print()
             print(cmd_instance.details)
 
     def _display_version(self) -> None:
-        # TODO: Find the version
-        name = "<TODO: Name>"
-        version = "<TODO: Version>"
-
-        # Display it
-        print(f"{name} {version}")
+        assert self.version is not None, self.version
+        print(f"{self.nicename} {self.version}")
 
     def command(
         self,
         *,
-        name: Optional[str] = None,
+        name: str | None = None,
         aliases: Iterable[str] = [],
-        summary: Optional[str] = None,
-        details: Optional[str] = None,
+        summary: str | None = None,
+        details: str | None = None,
         parameters: Iterable[Parameter] = [],
     ):
         """
         Register a function as a command, allowing users to call the function
         from the CLI. The function's name will be used as the command's name.
         """
 
@@ -248,15 +275,15 @@
 
         if details is not None:
             details = common.multiline_strip(details)
 
         parameters = list(parameters)
 
         # Create the decorator
-        def result(func: Callable) -> Callable:
+        def result(func: Callable[P, R]) -> Callable[P, R]:
             # Parse all parameters this function has
             parsed_parameters = {
                 params[0].name: params[0]
                 for params in argument_parser.parameters_from_function(func)
             }
 
             # Make sure the user-provided parameters match the function's
@@ -265,30 +292,32 @@
                     raise ValueError(
                         f"This function has no parameter named `{uparam.name}`"
                     )
 
             # Register the command
             self._commands.append(
                 AppCommand(
-                    name=common.python_name_to_console(func.__name__)
-                    if name is None
-                    else name,
+                    name=(
+                        common.python_name_to_console(func.__name__)
+                        if name is None
+                        else name
+                    ),
                     aliases=set(aliases),
                     summary=summary,
                     details=details,
                     function=func,
                     user_provided_parameters=parameters,
                 )
             )
 
             return func
 
         return result
 
-    def run(self, args: Optional[Iterable[str]] = None) -> None:
+    def run(self, args: Iterable[str] | None = None) -> None:
         if args is None:
             args = sys.argv[1:]
         else:
             args = list(args)
 
         # Which command should be run?
         #
@@ -306,14 +335,15 @@
         try:
             command_name, args = argument_parser.parse_function_name(
                 function_names=function_names,
                 function_aliases=function_aliases,
                 function_summaries=function_summaries,
                 raw_args=args,
                 interactive=True,
+                option_name="command",
             )
 
         # The user has cancelled the command
         except KeyboardInterrupt:
             print()
             print("[yellow]Canceled[/]")
             sys.exit(1)
@@ -334,28 +364,29 @@
         parser_params = [param[1] for param in param_pairs]
 
         for parser_param, user_param in zip(
             parser_params, command.user_provided_parameters
         ):
             parser_param.prompt = user_param.prompt
 
-        # Parse the parameters for the command
+        # Parse & run the command. These can easily fail, so catch exceptions.
         try:
+            # Parse the parameters for the command
             by_position_args, by_name_args = argument_parser.parse_function_parameters(
                 parser_params,
                 args,
                 interactive=True,
             )
 
+            # Call the command
+            command.function(*by_position_args, **by_name_args)
+
         # The user has cancelled the command
         except KeyboardInterrupt:
             print()
             print("[yellow]Canceled[/]")
             sys.exit(1)
 
         # Invalid Arguments
         except ArgumentError as err:
             error(err.message)
             sys.exit(1)
-
-        # Call the command
-        command.function(*by_position_args, **by_name_args)
```

### Comparing `revel-0.8.9/revel/common.py` & `revel-0.9.0/revel/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import *  # type: ignore
 
 from . import errors
 
 
 def comma_separated_list(
     values: Iterable[str],
-    conjunction: Optional[str],
-    quote: Optional[str],
+    conjunction: str | None,
+    quote: str | None,
 ) -> str:
     """
     Given a list of values, return a human-readable list of them. If the list
     contains only one value, that value is returned. Otherwise, the values are
     joined with commas, and the conjunction is inserted before the last value.
 
     The list is a comma-separated list of the values, with the conjunction
@@ -39,77 +39,88 @@
     if conjunction is None:
         return ", ".join(values[:-1])
     else:
         return ", ".join(values[:-1]) + " " + conjunction + " " + values[-1]
 
 
 def choose_string(
-    choices: Iterable[List[str]],
+    options: Sequence[str | list[str]],
     selection: str,
 ) -> int:
     """
     Given a list of choices and user input, find the choice the user wanted to
     select. This is a best-effort method, which does it's best to give the user
     leeway in what they type, without accidentally selecting an option they
     didn't want to select.
 
     If the function is confident in what the user wanted to select, it returns
     the index of the choice. Otherwise, it raises an exception.
 
-    Raises:
-        NoSuchOptionError: If the user's input doesn't match any of the
-            choices.
-        AmbiguousOptionError: If the user's input matches multiple choices.
+    ## Raises
+
+    `NoSuchOptionError`: If the user's input doesn't match any of the choices.
+
+    `AmbiguousOptionError`: If the user's input matches multiple choices.
     """
     # TODO: This method needs a lot of improvement. Consider using some sort of
-    # scoring system to determine which choice is the best match. For example,
-    # if an option starts with the user's choice, it should get priority over
-    # one that only contains it. It also currently cannot distinguish between
-    # uppercase and lowercase inputs.
+    # scoring system to determine which choice is the best match. It also
+    # currently cannot distinguish between uppercase and lowercase inputs.
+    #
+    # - exact match over wrong case
+    # - starts with over contains
+    # - consider user's uppercase as uppercase, but lowercase as undecided
+    # - ...
     #
     # Error reporting could also be better.
+    #
+    # I'll shut up now.
 
-    choices = list(choices)
+    # Expand the options
+    expanded_options: list[list[str]] = [
+        [option] if isinstance(option, str) else option for option in options
+    ]
+
+    # Normalize the user input
     selection = selection.strip().lower()
 
+    # Find all choices that match the user's input. If one matches exactly, go
+    # with that.
     matching_indices: Set[int] = set()
     matching_values: Set[str] = set()
 
-    # Find all choices that match the user's input. If one matches exactly, go
-    # with that.
-    for ii, choice_set in enumerate(choices):
+    for ii, choice_set in enumerate(expanded_options):
         for choice in choice_set:
             choice = choice.strip().lower()
 
             # Exact match? This is it
             if choice == selection:
                 return ii
 
             # Partial match? Add it to the list of possible matches
             if selection in choice:
                 matching_indices.add(ii)
                 matching_values.add(choice)
 
     # If there are no matches, return an error message
     if not matching_indices:
-        raise errors.NoSuchOptionError(selection, [x[0] for x in choices])
+        raise errors.NoSuchOptionError(selection, [x[0] for x in expanded_options])
 
     # If there is only one match, return it
     if len(matching_indices) == 1:
         return next(iter(matching_indices))
 
     # If there are multiple matches, return an error message
     raise errors.AmbiguousOptionError(
         selection,
         list(matching_values),
-        [x[0] for x in choices],
+        [x[0] for x in expanded_options],
     )
 
 
-def python_name_to_console(name: str) -> str:
+def python_name_to_console(name: str) -> str:  #
     """
     Convert a name as it would be used in Python to how it would be used in the
     console. For example, `foo_bar` becomes `foo-bar`.
     """
     name = name.strip("_")
     name = name.replace("_", "-")
     return name
@@ -139,7 +150,17 @@
     value = re.sub(
         r"\n+",
         lambda match: " " if match.group(0) == "\n" else "\n\n",
         value,
     )
 
     return value
+
+
+def an(noun: str) -> str:
+    """
+    Given a noun, return the correct indefinite article to use before it.
+    """
+    if noun[0].lower() in "aeiou":
+        return "an"
+    else:
+        return "a"
```

### Comparing `revel-0.8.9/revel/errors.py` & `revel-0.9.0/revel/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import *  # type: ignore
 
 from . import common
 
+__all__ = [
+    "RevelError",
+    "NoOptionGivenError",
+    "NoSuchOptionError",
+    "AmbiguousOptionError",
+    "ArgumentError",
+]
+
 
 @dataclass
 class RevelError(Exception, ABC):
     """Base class for all Revel exceptions."""
 
     @property
     @abstractmethod
@@ -16,44 +24,42 @@
         raise NotImplementedError
 
 
 @dataclass
 class NoOptionGivenError(RevelError):
     """Raised when the user doesn't specify a command."""
 
-    available_commands: List[str]
+    available_options: list[str]
 
-    @property
-    def message(self) -> str:
-        return f"Please specify a command. Available commands are {common.comma_separated_list(self.available_commands, 'and', '`')}."
+    def message(self, *, option_name: str = "option") -> str:
+        an = common.an(option_name)
+        return f"Please specify {an} {option_name}. Possible options are {common.comma_separated_list(self.available_options, 'and', '`')}."
 
 
 @dataclass
 class NoSuchOptionError(RevelError):
     """Raised when the user passes an invalid option."""
 
-    entered_command: str
-    available_commands: List[str]
+    entered_option: str
+    available_options: list[str]
 
-    @property
-    def message(self) -> str:
-        return f"`{self.entered_command}` is not a valid option."
+    def message(self, *, option_name: str = "option") -> str:
+        return f"`{self.entered_option}` is not a valid {option_name}."
 
 
 @dataclass
 class AmbiguousOptionError(RevelError):
     """Raised when the user passes an ambiguous option."""
 
-    entered_command: str
-    matching_commands: List[str]
-    available_commands: List[str]
+    entered_option: str
+    matching_options: list[str]
+    available_options: list[str]
 
-    @property
-    def message(self) -> str:
-        return f"`{self.entered_command}` is ambiguous. It could refer to {common.comma_separated_list(self.matching_commands, 'or', '`')}."
+    def message(self, *, option_name: str = "option") -> str:
+        return f"`{self.entered_option}` is ambiguous. It could refer to {common.comma_separated_list(self.matching_options, 'or', '`')}."
 
 
 class ArgumentError(RevelError):
     """
     Raised when attempting to call a function with invalid arguments. The
     message is human-readable and meant to be directly passed to the user
     """
```

### Comparing `revel-0.8.9/revel/legacy.py` & `revel-0.9.0/revel/legacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
+
 import atexit
 import enum
 import io
 import sys
 import time
 import typing
 from abc import ABC, abstractmethod
 from datetime import timedelta
-from sys import stdin, stdout
 from typing import *  # type: ignore
 
 import blessed
 import readchar
 
 from . import markup as markup_module
 from .style import Back, Fore, Format
@@ -40,18 +41,20 @@
 mode = _detect_mode()
 
 T = TypeVar("T")
 _SENTINEL = object()
 _py_input = input
 
 # Keep track of global state
-_docked_widget: Optional["Widget"] = None
-_chapter: Optional[str] = None
+_docked_widget: Widget | None = None
+_chapter: str | None = None
+
+
+# True, if nothing else has ever been printed
 _is_first_line = True
-_is_in_new_line = True
 
 # The position of the leftmost character in each line. This is 0 if outside of
 # chapters, and higher if inside a chapter
 _start_x: int = 0
 
 
 _KEY_NAMES = {
@@ -206,62 +209,48 @@
 
     # Translate special characters and return
     return _KEY_NAMES.get(key, key)
 
 
 class Widget(ABC):
     def __init__(self):
-        self._parent: Optional[Widget] = None
+        pass
 
     def mark_dirty(self) -> None:
         """
         Mark this widget as dirty, requesting a redraw.
         """
 
-        # If this widget has a parent, let that handle the call instead
-        if self._parent is not None:
-            self._parent.mark_dirty()
-            return
-
         # The widget isn't docked, there is nothing it can do
         if not self.is_docked:
             return
 
         # Redraw
         term = blessed.Terminal()
-        stdout.write(term.clear_bol())  # type: ignore
-        stdout.write(term.move_x(_start_x))
+        sys.stdout.write(term.clear_eol())
+        sys.stdout.write(term.move_x(_start_x))
         self.draw(term)
+        sys.stdout.write(term.move_x(0))
 
     @property
     def is_docked(self) -> bool:
         """
         Returns `True` if this widget is currently docked and `False` otherwise.
         """
         return self is _docked_widget
 
     def undock(self) -> None:
         global _docked_widget
         if _docked_widget is not self:
             raise ValueError("Widget is not docked")
 
         _docked_widget = None
-        self.on_undock()
 
-    def on_dock(self) -> None:
-        """
-        Called whenever a widget is being docked.
-        """
-        pass
-
-    def on_undock(self) -> None:
-        """
-        Called whenever a widget is being undocked.
-        """
-        pass
+        sys.stdout.write("\n")
+        sys.stdout.flush()
 
     @abstractmethod
     def draw(self, term: blessed.Terminal) -> None:
         """
         Draw the widget. The curser is at the top left position of the widget.
 
         TODO: Where should the cursor be after the widget is drawn?
@@ -289,19 +278,19 @@
     @text.setter
     def text(self, value: Any) -> None:
         self._text = str(value)
         self.mark_dirty()
 
     def draw(self, term: blessed.Terminal) -> None:
         if self.markup:
-            stdout.write(markup_module.unescape(self.text))
+            sys.stdout.write(markup_module.unescape(self.text))
         else:
-            stdout.write(self.text)
+            sys.stdout.write(self.text)
 
-        stdout.flush()
+        sys.stdout.flush()
 
 
 class Unit(enum.Enum):
     """
     Internal class for representing a unit.
     """
 
@@ -322,15 +311,15 @@
             return cls.TIME
         else:
             raise ValueError(f"Unknown unit type: {value}")
 
     def __str__(self) -> str:
         return self.name.lower()
 
-    def _units(self) -> Iterable[Tuple[str, float, bool]]:
+    def _units(self) -> Iterable[tuple[str, float, bool]]:
         """
         Return names of all units for this type and the divisor to convert from
         the base unit to them. The results are ordered from smallest to largest.
         In addition, a boolean is also returned, which indicates whether this
         unit is favorable (i.e. not an outdated or otherwise undesirable unit).
         """
 
@@ -363,15 +352,15 @@
             yield "hour", 60 * 60, True
             yield "d", 60 * 60 * 24, False
             yield "day", 60 * 60 * 24, True
 
         else:
             raise NotImplementedError(f"Unknown unit type: {self}")
 
-    def pretty_approximate_value(self, value: Union[int, float]) -> str:
+    def pretty_approximate_value(self, value: int | float) -> str:
         # Count: there is nothing to do here
         if self == Unit.COUNT:
             return str(round(value))
 
         # Time: This is a special case, because multiple units are used in the
         # result
         if self == Unit.TIME:
@@ -469,44 +458,48 @@
 
     _progress: float
     _width: int
     _unit: Unit
 
     def __init__(
         self,
-        progress: Union[int, float] = 0.0,
-        max: Union[int, float] = 1.0,
+        progress: int | float = 0.0,
+        max: int | float = 1.0,
         width: int = 50,
-        unit: Literal["count", "percent", "byte", "time"] = "percent",
+        unit: Literal["count", "percent", "byte", "time"] | None = None,
     ):
         super().__init__()
 
         # Data used to predict an ETA. This is a list of (timestamp, progress)
         # tuples, with `progress` being in range [0, 1]
-        self._progress_timestamps: List[Tuple[float, float]] = []
+        self._progress_timestamps: list[tuple[float, float]] = []
 
         self._last_update_time: float = 0.0
         self._last_update_fraction = self._calc_fraction(progress, max)
 
         self.max = max  # The `progress` setter uses this value, set it first
         self.progress = progress
         self.width = width
-        self.unit = unit
+
+        if unit is None:
+            self.unit = "count" if isinstance(progress, int) else "percent"
+        else:
+            self.unit = unit
 
     @property
-    def progress(self) -> Union[int, float]:
+    def progress(self) -> int | float:
         """
         How far the progress bar is filled. A value of 0 means that the bar is
         empty, while a value of `bar.max` means that the bar is completely
         filled.
         """
         return self._progress
 
     @progress.setter
-    def progress(self, value: Union[int, float]) -> None:
+    def progress(self, value: int | float) -> None:
         if not isinstance(value, (int, float)):
             raise TypeError("The progressbar's progress must be an integer or float")
 
         self._progress = value
 
         # Trigger a redraw, but only if necessary. For quick tasks, updating the
         # progressbar can be orders of magnitude more expensive than the task
@@ -537,22 +530,22 @@
             ):
                 del self._progress_timestamps[0]
 
             if len(self._progress_timestamps) > 100:
                 self._progress_timestamps = self._progress_timestamps[::2]
 
     @property
-    def max(self) -> Union[int, float]:
+    def max(self) -> int | float:
         """
         The value at which the bar is considered completely filled.
         """
         return self._max
 
     @max.setter
-    def max(self, value: Union[int, float]) -> None:
+    def max(self, value: int | float) -> None:
         if not isinstance(value, (int, float)):
             raise TypeError("The progressbar's maximum value must be a float")
 
         if value < 0:
             raise ValueError("The progressbar's maximum value cannot be negative")
 
         self._max = value
@@ -618,15 +611,15 @@
         # Set the progress to the maximum value
         self.progress = self.max
 
         if self.is_docked:
             self.undock()
 
     @property
-    def eta(self) -> Optional[timedelta]:
+    def eta(self) -> timedelta | None:
         """
         The estimated time until the progress bar is complete, or `None` if
         there is not enough data to calculate an ETA with reasonable confidence.
         """
         # Not enough data
         if not self._progress_timestamps or len(self._progress_timestamps) < 3:
             return None
@@ -671,151 +664,147 @@
         # Empty blocks
         bar_string += n_blocks_remaining * blocks[0]
 
         return bar_string
 
     def draw(self, term: blessed.Terminal) -> None:
         # Display the bar
-        stdout.write(markup_module.unescape(self.bar_string))
+        sys.stdout.write(markup_module.unescape(self.bar_string))
 
         # Display written progress
         unit = Unit.from_string(self.unit)  # type: ignore
         fraction = self.fraction
 
         if unit == Unit.PERCENT:
-            stdout.write(f" {fraction*100:.1f}%")
+            sys.stdout.write(f" {fraction*100:.1f}%")
         elif unit == Unit.TIME:
             if fraction != 1:
-                stdout.write(
+                sys.stdout.write(
                     f"  {unit.pretty_approximate_value(self.max - self.progress)}"
                 )
         elif fraction == 1:
-            stdout.write(f"  {unit.pretty_approximate_value(self.max)}")
+            sys.stdout.write(f"  {unit.pretty_approximate_value(self.max)}")
         else:
-            stdout.write(
+            sys.stdout.write(
                 f"  {unit.pretty_approximate_value(self.progress)} ╱ {unit.pretty_approximate_value(self.max)}"
             )
 
         # Display an ETA
         if fraction != 1:
             eta = self.eta
             if eta is not None:
                 pretty_str = Unit.TIME.pretty_approximate_value(eta.total_seconds())
-                stdout.write(
+                sys.stdout.write(
                     markup_module.unescape(
                         f"[bright_black] — about {pretty_str} remaining[/]"
                     )
                 )
 
-        stdout.flush()
+        sys.stdout.flush()
 
     def __enter__(self) -> "ProgressBar":
         print(self, dock=True)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.complete()
 
 
-def get_docked_widget() -> Optional[Widget]:
+def get_docked_widget() -> Widget | None:
     """
     Returns the currently docked widget, or `None` if no widget is docked.
     """
     return _docked_widget
 
 
-def _print_newline(n_newlines: int = 1) -> None:
-    global _is_in_new_line
-    assert n_newlines >= 0, n_newlines
-
-    if n_newlines == 0:
-        return
-
-    if _is_in_new_line:
-        n_newlines -= 1
-
-    stdout.write("\n" * n_newlines)
-    _is_in_new_line = False
-
-
 Tprint = TypeVar("Tprint", bound=Widget)
 
 
 @typing.overload
-def print(*values: Tprint, dock: bool = False, markup: bool = True) -> Tprint:
-    ...
+def print(*values: Tprint, dock: bool = False, markup: bool = True) -> Tprint: ...
 
 
 @typing.overload
-def print(*values: Any, dock: bool = False, markup: bool = True) -> TextLine:
-    ...
+def print(*values: Any, dock: bool = False, markup: bool = True) -> TextLine: ...
 
 
 def print(*values: Any, dock: bool = False, markup: bool = True) -> Widget:
     """
     Prints a widget to the terminal, optionally docking it.
 
     If a single widget is passed it is returned, otherwise the inputs are
     converted to strings, joined with a space and returned as a `TextLine`.
     """
-    global _docked_widget, _is_first_line, _is_in_new_line
+    global _docked_widget, _is_first_line
 
     # Convert the inputs to a single Widget
     if len(values) == 1 and isinstance(values[0], Widget):
         widget = values[0]
     else:
         widget = TextLine(
             " ".join(str(v) for v in values),
             markup=markup,
         )
 
-    # Position the cursor at the start of a new line, taking any docked widgets
-    # into account
+    # Depending on whether this widget is being docked and whether another
+    # widget is already docked, one or more widgets may have to be drawn into
+    # account
     term = blessed.Terminal()
-    other_docked_widget_remains_below = _docked_widget is not None and not dock
 
-    if other_docked_widget_remains_below:
-        stdout.write(term.clear_bol)  # Clear to the start of the line
-    elif dock:
-        if _docked_widget is not None:
-            _docked_widget.on_undock()
-
-        widget.on_dock()
+    if _docked_widget is None and not dock:
+        sys.stdout.write(term.move_x(_start_x))
+        widget.draw(term)
+        sys.stdout.write("\n")
+    elif _docked_widget is None and dock:
         _docked_widget = widget
 
-        _print_newline()
+        sys.stdout.write(term.move_x(_start_x))
+        widget.draw(term)
+        sys.stdout.write(term.move_x(0))
+    elif _docked_widget is not None and not dock:
+        sys.stdout.write(term.clear_eol())
+        sys.stdout.write(term.move_x(_start_x))
+        widget.draw(term)
+        sys.stdout.write("\n")
+
+        sys.stdout.write(term.move_x(_start_x))
+        _docked_widget.draw(term)
+        sys.stdout.write(term.move_x(0))
     else:
-        _print_newline()
+        assert _docked_widget is not None
 
-    # Display the widget
-    stdout.write(term.move_x(_start_x))
-    widget.draw(term)
+        _docked_widget = widget
+        sys.stdout.write("\n")
+        sys.stdout.write(term.move_x(_start_x))
+        widget.draw(term)
+        sys.stdout.write(term.move_x(0))
 
-    # Re-display the docked widget
-    if other_docked_widget_remains_below:
-        assert _docked_widget is not None
-        _print_newline()
-        stdout.write(term.move_x(_start_x))
-        _docked_widget.draw(term)
+    sys.stdout.flush()
 
     # Update global state
     _is_first_line = False
-    _is_in_new_line = False
 
     return widget
 
 
 def _basic_print(prefix: str, values: Iterable[Any], markup: bool) -> None:
     values = " ".join(map(str, values))
     if not markup:
         values = markup_module.escape(values)
 
     print(f"{prefix}{values}", dock=False)
 
 
+def debug(*values: Any, markup: bool = True) -> None:
+    """
+    Displays a debug message, highlighted to draw attention to it.
+    """
+    _basic_print("[cyan]", values, markup)
+
+
 def success(*values: Any, markup: bool = True) -> None:
     """
     Displays a success message, highlighted to draw attention to it.
     """
     # This differs from the other, similar functions, because prefixing the text
     # with 'success' looks oddly stupid.
     _basic_print("[green]", values, markup)
@@ -840,61 +829,61 @@
     Displays an error message, highlighted to draw attention to it, and then
     exits the program.
     """
     _basic_print("[bold][red]ERROR:[/bold] ", values, markup)
     sys.exit(status_code)
 
 
-def print_chapter(name: Optional[str]) -> None:
+def print_chapter(name: str | None) -> None:
     """
     Displays a chapter heading. Chapters are highlighted and create whitespace
     to visually separate them from other widgets.
     """
 
-    global _docked_widget, _is_first_line, _chapter, _is_in_new_line, _start_x
+    global _docked_widget, _is_first_line, _chapter, _start_x
 
     # Undock any previously docked widgets
     if _docked_widget is not None:
-        _docked_widget.on_undock()
         _docked_widget = None
+        sys.stdout.write("\n")
 
     # Spacing to previous content
     if not _is_first_line:
-        _print_newline(1)
+        sys.stdout.write("\n")
 
     # Print the chapter name
     if name is None:
         _start_x = 0
     else:
-        _print_newline(1)
-        stdout.write(
-            markup_module.unescape(f"[bold primary] > {markup_module.escape(name)}[/]")
-        )
         _start_x = 3
+        sys.stdout.write(
+            markup_module.unescape(
+                f"[bold primary] > {markup_module.escape(name)}[/]\n"
+            )
+        )
 
-    stdout.flush()
+    sys.stdout.flush()
 
     # Update global state
-    _chapter = name
     _is_first_line = False
-    _is_in_new_line = False
+    _chapter = name
 
 
 def _secret_input() -> str:
     """
-    Get input from `stdin`, displaying an asterisk for each character.
+    Get input from `sys.stdin`, displaying an asterisk for each character.
     """
     result = ""
     while True:
         # Get a key
         ch = input_key()
 
         # Done?
         if ch == "\r" or ch == "\n":
-            _print_newline()
+            sys.stdout.write("\n")
             return result
 
         # Backspace
         if ch == "backspace":
             if result:
                 result = result[:-1]
                 sys.stdout.write("\b \b")
@@ -915,41 +904,38 @@
 def input(
     prompt: str = "",
     *,
     sep: str = " > ",
     parse: Callable[[str], T] = str,
     markup: bool = True,
     secret: bool = False,
-) -> T:
-    ...
+) -> T: ...
 
 
 @typing.overload
 def input(
     *,
     default: T,
     sep: str = " > ",
     parse: Callable[[str], T] = str,
     markup: bool = True,
     secret: bool = False,
-) -> T:
-    ...
+) -> T: ...
 
 
 @typing.overload
 def input(
     prompt: str,
     default: T,
     *,
     sep: str = " > ",
     parse: Callable[[str], T] = str,
     markup: bool = True,
     secret: bool = False,
-) -> T:
-    ...
+) -> T: ...
 
 
 def input(
     prompt: str = "",
     default: T = _SENTINEL,
     *,
     sep: str = " > ",
@@ -960,43 +946,45 @@
     """
     Asks the user for a value and returns it. If `prompt` is given, it is
     displayed first. `parse` is applied to the user's input, and its result
     returned. If `parse` raises a `ValueError` the user is asked for another
     value. Lastly, if `default` is given, it is returned if the user enters an
     empty string.
     """
-    global _is_in_new_line
+    global _is_first_line
+
+    # Update global state
+    _is_first_line = False
 
     # Undock any existing widget
     if _docked_widget is not None:
         _docked_widget.undock()
+        sys.stdout.write("\n")
 
     # Preprocess the prompt
     if markup:
         prompt = markup_module.unescape(prompt)
 
     prompt += markup_module.unescape(f"[primary bold]{markup_module.escape(sep)}[/]")
 
     if _chapter is not None:
         prompt = f"   {prompt}"
 
     # Ask for values, until a valid one comes along
     while True:
         # Get a value
         if secret:
-            _print_newline()
-            stdin.flush()
             sys.stdout.write(prompt)
             sys.stdout.flush()
+            sys.stdin.flush()
             value = _secret_input()
         else:
             _set_echo(True)
             _set_cursor(True)
-            _print_newline()
-            stdin.flush()
+            sys.stdin.flush()
             try:
                 value = _py_input(prompt).strip()
             finally:
                 _set_echo(False)
                 _set_cursor(False)
 
         # Use the default value?
@@ -1005,29 +993,41 @@
 
         # Try to parse it, thus verifying it's valid
         try:
             value = parse(value)
         except ValueError:
             continue
 
-        # The user has just pressed `enter`, so the cursor is in a new line
-        _is_in_new_line = True
-
         return value
 
 
 def select_short(
     prompt: str,
-    options: Dict[str, Any],
+    options: dict[str, Any],
     *,
-    default_str: Optional[str] = None,
+    default_str: str | None = None,
     add_yes_no_options: bool = False,
 ) -> Any:
     """
-    TODO
+    Allows the user to choose between a set of options. The options are expected
+    to be few and short, as they're styled in a single line.
+
+    ## Args
+
+    `prompt`: The question to ask the user.
+
+    `options`: A dictionary mapping the user's input to the corresponding value.
+    This value will be returned should the user select the option.
+
+    `default_str`: The default option, as a string. If the user enters an empty
+    string, this option is returned. If `None`, there is no default option. The
+    user will be forced to enter a valid option in this case.
+
+    `add_yes_no_options`: If `True` the available options will be padded with
+    common yes/no options, such as "y", "true", "y", etc.
     """
     for opt in options.keys():
         assert opt == opt.lower(), opt
 
     # Prepared, commonly used options
     if add_yes_no_options:
         t = {
@@ -1079,19 +1079,20 @@
 
         try:
             return options[response]
         except KeyError:
             pass
 
         # Ask again if it's invalid
-        _print_newline()
-        sys.stdout.write(f"Please respond with one of {options_string}")
+        sys.stdout.write("\n")
+        sys.stdout.write(f"Please respond with one of {options_string}\n")
+        sys.stdout.flush()
 
 
-def select_yes_no(prompt: str, default_value: Optional[bool] = None) -> bool:
+def select_yes_no(prompt: str, default_value: bool | None = None) -> bool:
     """
     Displays the prompt to the user, and returns True if the user responds with
     yes, and False if the user responds with no. If no input is entered and a
     default value is provided it is returned instead.
 
     The function makes a best effort to interpret the user's input, and will
     accept a variety of possible values.
@@ -1111,39 +1112,42 @@
     )
 
 
 def _set_echo(enable_echo: bool):
     if mode != "terminal" or termios is None:
         return  # TODO
 
-    fd = sys.stdin.fileno()
-    (iflag, oflag, cflag, lflag, ispeed, ospeed, cc) = termios.tcgetattr(fd)
+    # termios doesn't work in some environemnts, such as cron
+    try:
+        fd = sys.stdin.fileno()
+        (iflag, oflag, cflag, lflag, ispeed, ospeed, cc) = termios.tcgetattr(fd)
 
-    if enable_echo:
-        lflag |= termios.ECHO
-    else:
-        lflag &= ~termios.ECHO
+        if enable_echo:
+            lflag |= termios.ECHO
+        else:
+            lflag &= ~termios.ECHO
 
-    new_attr = [iflag, oflag, cflag, lflag, ispeed, ospeed, cc]
-    termios.tcsetattr(fd, termios.TCSANOW, new_attr)
+        new_attr = [iflag, oflag, cflag, lflag, ispeed, ospeed, cc]
+        termios.tcsetattr(fd, termios.TCSANOW, new_attr)
+    except (termios.error, io.UnsupportedOperation):
+        pass
 
 
 def _set_cursor(enable_cursor: bool):
     if mode != "terminal":
         return
 
-    stdout.write("\033[?25h" if enable_cursor else "\033[?25l")
-    stdout.flush()
+    sys.stdout.write("\033[?25h" if enable_cursor else "\033[?25l")
+    sys.stdout.flush()
 
 
 def _on_exit():
     # Clean up the terminal
     if mode == "terminal":
         _set_echo(True)
         _set_cursor(True)
-        stdout.write("\n")
-        stdout.flush()
+        sys.stdout.flush()
 
 
 atexit.register(_on_exit)
 _set_echo(False)
 _set_cursor(False)
```

### Comparing `revel-0.8.9/revel/markup.py` & `revel-0.9.0/revel/markup.py`

 * *Files identical despite different names*

### Comparing `revel-0.8.9/revel/menu.py` & `revel-0.9.0/revel/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import sys
 from abc import ABC, abstractmethod
 from typing import *  # type: ignore
 
 import blessed
 
-from revel.legacy import _print_newline
-
 from . import legacy
 from . import markup as markup_module
 
 T = TypeVar("T")
 
 
 class Menu(ABC):
@@ -55,17 +53,14 @@
         sys.stdout.write(self.term.move_down * offset)
         sys.stdout.write(self.term.move_x(0))
         sys.stdout.flush()
 
     def run(self, prompt: str) -> None:
         previous_index = 0
 
-        # Make sure this is is on a newline
-        _print_newline()
-
         # Display the prompt
         if prompt:
             sys.stdout.write(self.term.move_x(legacy._start_x))
             sys.stdout.write(markup_module.unescape(prompt))
             sys.stdout.write("\n\n")
 
         # Display the initial menu
@@ -73,14 +68,15 @@
             sys.stdout.write(self.term.move_x(legacy._start_x))
             self.draw_line(index)
             sys.stdout.write("\n")
 
         sys.stdout.write("\n")
         sys.stdout.write(self.term.move_x(legacy._start_x))
         sys.stdout.write(markup_module.unescape(self.footer))
+        sys.stdout.write(self.term.move_x(0))
         sys.stdout.flush()
 
         # Hand control to the user
         with self.term.cbreak(), self.term.hidden_cursor():
             while True:
                 previous_index = self.current_index
 
@@ -107,15 +103,15 @@
                 if self.current_index != previous_index:
                     self.on_move_up_or_down(previous_index)
 
         assert False, "Should never get here"
 
 
 class SingleSelectMenu(Menu):
-    def __init__(self, options: List[str]):
+    def __init__(self, options: list[str]):
         super().__init__(
             n_options=len(options),
             footer=f"[dim]⇅ or 1-{min(9, len(options))} to move, ↩ to confirm[/dim]",
         )
         self.options = options
 
     def draw_line(self, index: int) -> None:
@@ -149,15 +145,15 @@
         return False
 
     def on_move_up_or_down(self, previous_index: int) -> None:
         self.force_redraw_line(previous_index)
         self.force_redraw_line(self.current_index)
 
 
-def select(options: Dict[str, T], *, prompt: str = "") -> T:
+def select(options: dict[str, T], *, prompt: str = "") -> T:
     """
     Asks the user to select one of the given options. If `prompt` is given, it
     is displayed first. The options are displayed as a numbered list, and the
     user is asked to select one of them.
     """
 
     if not options:
@@ -171,22 +167,22 @@
     # Return the selected option
     return opt_list[menu.current_index][1]
 
 
 class MultiSelectMenu(Menu):
     def __init__(
         self,
-        options: List[str],
+        options: list[str],
     ):
         super().__init__(
             n_options=len(options) + 1,
             footer=f"[dim]Use ⇅ to move, ␣ space to select, ↩ to confirm[/dim]",
         )
-        self.options: List[str] = options
-        self.checked: List[bool] = [False] * len(options)
+        self.options: list[str] = options
+        self.checked: list[bool] = [False] * len(options)
 
     def draw_line(self, index: int) -> None:
         is_selected = index == self.current_index
 
         # Is this the "Done" option?
         if index == self.n_options - 1:
             if is_selected:
@@ -225,17 +221,19 @@
         return False
 
     def on_move_up_or_down(self, previous_index: int) -> None:
         self.force_redraw_line(previous_index)
         self.force_redraw_line(self.current_index)
 
 
-def select_multiple(options: Dict[str, T], *, prompt: str = "") -> List[T]:
+def select_multiple(options: dict[str, T], *, prompt: str = "") -> list[T]:
     """
-    TODO
+    Allows the user to choose between a set of options. A menu will be displayed
+    on the screen with all the options, and the user can select multiple options
+    by toggling them on and off.
     """
 
     if not options:
         raise ValueError("Please provide at least one option")
 
     # Delegate to the interactive menu class
     opt_list = list(options.items())
```

### Comparing `revel-0.8.9/revel/rapidbaby/parser.py` & `revel-0.9.0/revel/rapidbaby/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 TAG_PATTERN = re.compile(r"(?<!\[)(\[\[)*(\[/?[\w\- ]*\])")
 
 
 def prepare_plaintext_highlights() -> re.Pattern:
     raw = (
         (
             "url",
-            r"\bhttps?://[^\s/$.?#].[^\s]*\b",
+            r"\b(http|https|ftp|file)://[^\s/$.?#]+\.[^\s]+\b/?",
         ),
         (
             "email",
             r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}\b",
         ),
         (
             "number",
@@ -39,20 +39,20 @@
 
 class Baby:
     def __init__(self, styles: StyleSet):
         # All styles known to the parser
         self._styles = styles
 
         # Contains all partial results that have been processed so far
-        self._partial_results: List[str] = []
+        self._partial_results: list[str] = []
 
         # Contains all currently active styles, in the same order they were
         # applied. This is a list of sets, because a single tag can contain
         # multiple styles.
-        self._style_stack: List[Set[Style]] = []
+        self._style_stack: list[Set[Style]] = []
 
         # Counts how often each style is currently active.
         self._style_counter: Counter[str] = Counter()
 
         # Counts how often each style category is currently active
         self._category_counter: Counter[StyleCategory] = Counter()
```

### Comparing `revel-0.8.9/revel/rapidbaby/styles.py` & `revel-0.9.0/revel/rapidbaby/styles.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.stop_string = stop_string
         self.category = category
 
 
 class StyleSet:
     def __init__(self):
         # All known styles
-        self._styles: Dict[str, Set[Style]] = {}
+        self._styles: dict[str, Set[Style]] = {}
 
         # Add all fundamental styles
         self._register_fundamental_styles()
 
     def _register_fundamental_styles(self) -> None:
         self._add_fundamental_style(
             "bold",
@@ -174,15 +174,19 @@
             "bg-white",
             style.Back.WHITE,
             style.Back.RESET,
             StyleCategory.BACKGROUND_COLOR,
         )
 
     def _add_fundamental_style(
-        self, name: str, start_string: str, stop_string: str, category: StyleCategory
+        self,
+        name: str,
+        start_string: str,
+        stop_string: str,
+        category: StyleCategory,
     ) -> None:
         """
         Registers a new style.
         """
         assert name not in self._styles, name
         self._styles[name] = {
             Style(name, start_string, stop_string, category),
```

### Comparing `revel-0.8.9/revel/shell_escape.py` & `revel-0.9.0/revel/shell_escape.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __all__ = [
     "guess_shell",
     "shell_escape",
 ]
 
 
-_ACTIVE_SHELL: Optional[Literal["bourne", "cmd.exe", "powershell"]] = None
+_ACTIVE_SHELL: Literal["bourne", "cmd.exe", "powershell"] | None = None
 
 
 def _guess_shell_non_cached() -> Literal["bourne", "cmd.exe", "powershell"]:
     # If the SHELL environment variable is set, use that
     try:
         shell_var = os.environ["SHELL"]
     except KeyError:
```

### Comparing `revel-0.8.9/revel/style.py` & `revel-0.9.0/revel/style.py`

 * *Files identical despite different names*

### Comparing `revel-0.8.9/PKG-INFO` & `revel-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: revel
-Version: 0.8.9
+Version: 0.9.0
 Summary: Effortlessly spice up your terminal apps using colors, progressbars & more
+Home-page: https://gitlab.com/Vivern/revel
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: blessed (>=1.19.1,<2.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: readchar (>=4.0.3,<5.0.0)
+Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
+Project-URL: Repository, https://gitlab.com/Vivern/revel
 Description-Content-Type: text/markdown
 
 # Revel
 
 `revel` helps you create beautiful interfaces for your command line tools. Best
 of all, it's extremely easy to use.
```

