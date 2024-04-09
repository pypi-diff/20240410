# Comparing `tmp/doxtrings-0.1.1.tar.gz` & `tmp/doxtrings-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doxtrings-0.1.1.tar", last modified: Fri Jan 12 11:24:57 2024, max compression
+gzip compressed data, was "doxtrings-0.2.0.tar", last modified: Tue Apr  9 21:30:58 2024, max compression
```

## Comparing `doxtrings-0.1.1.tar` & `doxtrings-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0     1877 2023-09-13 12:34:59.475432 doxtrings-0.1.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0      601 2023-09-13 12:34:59.476359 doxtrings-0.1.1/.github/workflows/test_run.yaml
--rw-r--r--   0        0        0      767 2023-09-13 12:34:59.477339 doxtrings-0.1.1/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      369 2023-08-29 14:52:20.512479 doxtrings-0.1.1/.gitignore
--rw-r--r--   0        0        0      661 2024-01-12 11:23:19.052312 doxtrings-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      814 2023-08-29 15:42:41.581070 doxtrings-0.1.1/README.md
--rw-r--r--   0        0        0     2439 2023-08-29 15:42:41.582121 doxtrings-0.1.1/docs/contributing.md
--rw-r--r--   0        0        0      967 2023-08-29 11:49:51.187932 doxtrings-0.1.1/docs/gen_ref_pages.py
--rw-r--r--   0        0        0    59377 2023-08-29 15:42:41.583316 doxtrings-0.1.1/docs/img/logo.png
--rw-r--r--   0        0        0      699 2023-08-29 12:14:26.579822 doxtrings-0.1.1/docs/index.md
--rw-r--r--   0        0        0      148 2023-08-29 15:42:41.585034 doxtrings-0.1.1/docs/overrides/extra.css
--rw-r--r--   0        0        0      219 2023-08-29 15:42:41.587257 doxtrings-0.1.1/docs/overrides/templates/main.html
--rw-r--r--   0        0        0     6425 2023-12-10 21:27:58.787429 doxtrings-0.1.1/docs/start.md
--rw-r--r--   0        0        0     1518 2023-08-28 14:38:39.993463 doxtrings-0.1.1/docs/usage.md
--rw-r--r--   0        0        0      804 2023-09-13 12:34:59.478613 doxtrings-0.1.1/mkdocs.yaml
--rw-r--r--   0        0        0     1431 2023-12-12 11:49:55.292083 doxtrings-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       84 2024-01-12 11:23:31.580952 doxtrings-0.1.1/src/doxtrings/__init__.py
--rw-r--r--   0        0        0       99 2023-08-02 19:11:49.820269 doxtrings-0.1.1/src/doxtrings/cli/__init__.py
--rw-r--r--   0        0        0     1042 2023-08-05 18:25:05.266120 doxtrings-0.1.1/src/doxtrings/cli/scan.py
--rw-r--r--   0        0        0    15769 2023-12-12 11:49:21.455639 doxtrings-0.1.1/src/doxtrings/config.py
--rw-r--r--   0        0        0      294 2023-08-02 19:34:51.029661 doxtrings-0.1.1/src/doxtrings/core/__init__.py
--rw-r--r--   0        0        0      149 2023-08-02 18:13:58.897078 doxtrings-0.1.1/src/doxtrings/core/parser/__init__.py
--rw-r--r--   0        0        0     6864 2023-08-15 20:33:56.670173 doxtrings-0.1.1/src/doxtrings/core/parser/file_parser.py
--rw-r--r--   0        0        0    27400 2024-01-12 11:23:48.635613 doxtrings-0.1.1/src/doxtrings/core/parser/node_parser.py
--rw-r--r--   0        0        0     3225 2023-12-12 11:50:26.320208 doxtrings-0.1.1/src/doxtrings/core/report.py
--rw-r--r--   0        0        0     2217 2023-08-02 14:36:42.535661 doxtrings-0.1.1/src/doxtrings/core/search.py
--rw-r--r--   0        0        0     2182 2023-08-15 20:24:17.648561 doxtrings-0.1.1/src/doxtrings/documentable.py
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 doxtrings-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1877 2023-09-13 12:34:59.475432 doxtrings-0.2.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      601 2023-09-13 12:34:59.476359 doxtrings-0.2.0/.github/workflows/test_run.yaml
+-rw-r--r--   0        0        0      767 2023-09-13 12:34:59.477339 doxtrings-0.2.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      369 2023-08-29 14:52:20.512479 doxtrings-0.2.0/.gitignore
+-rw-r--r--   0        0        0      661 2024-01-12 11:23:19.052312 doxtrings-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      814 2023-08-29 15:42:41.581070 doxtrings-0.2.0/README.md
+-rw-r--r--   0        0        0     2439 2023-08-29 15:42:41.582121 doxtrings-0.2.0/docs/contributing.md
+-rw-r--r--   0        0        0      967 2023-08-29 11:49:51.187932 doxtrings-0.2.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0    59377 2023-08-29 15:42:41.583316 doxtrings-0.2.0/docs/img/logo.png
+-rw-r--r--   0        0        0      699 2023-08-29 12:14:26.579822 doxtrings-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      148 2023-08-29 15:42:41.585034 doxtrings-0.2.0/docs/overrides/extra.css
+-rw-r--r--   0        0        0      219 2023-08-29 15:42:41.587257 doxtrings-0.2.0/docs/overrides/templates/main.html
+-rw-r--r--   0        0        0     6373 2024-04-09 21:29:30.744939 doxtrings-0.2.0/docs/start.md
+-rw-r--r--   0        0        0     1510 2024-04-09 21:29:30.745853 doxtrings-0.2.0/docs/usage.md
+-rw-r--r--   0        0        0      804 2023-09-13 12:34:59.478613 doxtrings-0.2.0/mkdocs.yaml
+-rw-r--r--   0        0        0     1423 2024-04-09 21:29:30.746952 doxtrings-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-09 21:29:30.748024 doxtrings-0.2.0/src/doxtrings/__init__.py
+-rw-r--r--   0        0        0       99 2023-08-02 19:11:49.820269 doxtrings-0.2.0/src/doxtrings/cli/__init__.py
+-rw-r--r--   0        0        0     1078 2024-04-09 21:29:30.748906 doxtrings-0.2.0/src/doxtrings/cli/scan.py
+-rw-r--r--   0        0        0      125 2024-04-09 21:29:30.750093 doxtrings-0.2.0/src/doxtrings/config/__init__.py
+-rw-r--r--   0        0        0     7158 2024-04-09 21:29:30.750901 doxtrings-0.2.0/src/doxtrings/config/builder.py
+-rw-r--r--   0        0        0     1455 2024-04-09 21:29:30.751639 doxtrings-0.2.0/src/doxtrings/config/merge.py
+-rw-r--r--   0        0        0     9689 2024-04-09 21:29:30.752287 doxtrings-0.2.0/src/doxtrings/config/models.py
+-rw-r--r--   0        0        0      294 2023-08-02 19:34:51.029661 doxtrings-0.2.0/src/doxtrings/core/__init__.py
+-rw-r--r--   0        0        0      149 2023-08-02 18:13:58.897078 doxtrings-0.2.0/src/doxtrings/core/parser/__init__.py
+-rw-r--r--   0        0        0     7298 2024-04-09 21:29:30.753313 doxtrings-0.2.0/src/doxtrings/core/parser/file_parser.py
+-rw-r--r--   0        0        0    28493 2024-04-09 21:29:30.754968 doxtrings-0.2.0/src/doxtrings/core/parser/node_parser.py
+-rw-r--r--   0        0        0     3338 2024-04-09 21:29:30.755914 doxtrings-0.2.0/src/doxtrings/core/report.py
+-rw-r--r--   0        0        0     2513 2024-04-09 21:29:30.756952 doxtrings-0.2.0/src/doxtrings/core/search.py
+-rw-r--r--   0        0        0     2182 2023-08-15 20:24:17.648561 doxtrings-0.2.0/src/doxtrings/documentable.py
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 doxtrings-0.2.0/PKG-INFO
```

### Comparing `doxtrings-0.1.1/.github/workflows/build.yaml` & `doxtrings-0.2.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/.github/workflows/test_run.yaml` & `doxtrings-0.2.0/.github/workflows/test_run.yaml`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/.github/workflows/tests.yaml` & `doxtrings-0.2.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/.pre-commit-config.yaml` & `doxtrings-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/README.md` & `doxtrings-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/docs/contributing.md` & `doxtrings-0.2.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/docs/gen_ref_pages.py` & `doxtrings-0.2.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/docs/img/logo.png` & `doxtrings-0.2.0/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/docs/index.md` & `doxtrings-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/docs/start.md` & `doxtrings-0.2.0/docs/start.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,84 +34,84 @@
 ### Example Configurations
 #### doXtrings Configuration Settings
 
 The doXtrings package employs its own capabilities to keep documentation up-to-date within its codebase. Below is the configuration utilized within the project:
 
 ```toml
 [tool.doxtrings]
-root_dir = "./src/doxtrings"
+path = "./src/doxtrings"
 
-[tool.doxtrings.ignore_filters.default]
+[tool.doxtrings.ignore_rules.default]
 ignore_prefixes_rules = ["_"]
 include_prefixes_rules = ["__init__"]
 
-[tool.doxtrings.ignore_filters.variables]
+[tool.doxtrings.ignore_rules.variables]
 ignore_matches = ["logger"]
 ```
 
 Alternatively, if not defined in `pyproject.toml`:
 
 ```toml
-root_dir = "./src/doxtrings"
+path = "./src/doxtrings"
 
-[ignore_filters.default]
+[ignore_rules.default]
 ignore_prefixes_rules = ["_"]
 include_prefixes_rules = ["__init__"]
 
-[ignore_filters.variables]
+[ignore_rules.variables]
 ignore_matches = ["logger"]
 ```
 
 Let's delve into the available options:
 
-1. `root_dir`: This option designates the root directory where doXtrings will search for files to parse.
-2. `ignore_filters`: This section configures rules for nodes that should be ignored during the parsing process.
-3. `ignore_filters.default`: Within this subsection, you can define rules that are common to all types of nodes in the codebase. The possible node types are: modules, classes, methods, functions, constants, attributes, and variables.
-4. `ignore_filters.default.ignore_prefixes_rules`: This rule instructs doXtrings to disregard any node beginning with `_`, effectively excluding private nodes from documentation.
-5. `ignore_filters.default.include_prefixes_rules`: In contrast to the previous rule, this directive overrides the former by including nodes that start with `__init__`. This is especially important for modules and methods named `__init__`, ensuring their documentation is not overlooked.
-6. `ignore_filters.variables`: This section enables the specification of ignore rules that exclusively apply to variables within the codebase.
-7. `ignore_filters.variables.ignore_matches`: Specifically, this rule will ignore the documentation of all variables named `logger`. It is a common practice to create a new logger in each file, and its usually not desired to document all of them.
+1. `path`: This option designates the root directory where doXtrings will search for files to parse.
+2. `ignore_rules`: This section configures rules for nodes that should be ignored during the parsing process.
+3. `ignore_rules.default`: Within this subsection, you can define rules that are common to all types of nodes in the codebase. The possible node types are: modules, classes, methods, functions, constants, attributes, and variables.
+4. `ignore_rules.default.ignore_prefixes_rules`: This rule instructs doXtrings to disregard any node beginning with `_`, effectively excluding private nodes from documentation.
+5. `ignore_rules.default.include_prefixes_rules`: In contrast to the previous rule, this directive overrides the former by including nodes that start with `__init__`. This is especially important for modules and methods named `__init__`, ensuring their documentation is not overlooked.
+6. `ignore_rules.variables`: This section enables the specification of ignore rules that exclusively apply to variables within the codebase.
+7. `ignore_rules.variables.ignore_matches`: Specifically, this rule will ignore the documentation of all variables named `logger`. It is a common practice to create a new logger in each file, and its usually not desired to document all of them.
 
  !!! Note
     An important feature to highlight is that, even if a node is ignored, it might still raise errors if it was incorrectly documented. Set `fail_ignored_if_incorrect` to `False` if you wish to completely ignore nodes.
 
 #### Lenient Example
 
 The previous configuration might feel a bit strict for many users. It asks you to document every module, class attribute, constant, and function. You also need to include type hints in the docstrings if you've used type hints in your function signature.
 
 A more relaxed approach is to document just classes, methods, and functions. Let's explore a sample configuration used in the deepFlow project:
 
 ```toml
-root_dir = "./src/deepflow"
+path = "./src/deepflow"
 types_to_check = ["class", "function", "method"]
 
-[ignore_filters.default]
+[ignore_rules.default]
 ignore_prefixes_rules = ["_"]  # Ignores private nodes
 ignore_typing = true
 ignore_args_and_kwargs = true
 
-[ignore_filters.modules]
+[ignore_rules.modules]
 ignore_prefixes_rules = []
 ```
 
 Here's what's different in this configuration:
 
 1. `types_to_check`: With this set, doxtrings examines only the nodes belonging to these specified types: classes, functions, and methods.
-2. `ignore_filters.default.ignore_typing`: You don't need to include type hints in the docstrings, though incorrect types will still cause failures.
-3. `ignore_filters.default.ignore_args_and_kwargs`: Documenting `*args` and `**kwargs` parameters in methods and functions isn't required.
-4. `ignore_filters.modules.ignore_prefixes_rules`: deepFlow follows a convention of writing most of the code in private modules and then reimporting the desired objects in the `__init__` module. Even though we are not checking the modules for the docstrings, we would still be ignoring the ones that start with `_` as it is a default ignore rule. Then, most of the code would simply be ignored (elements inside an ignored node are also ignored). Setting no ignore rules for modules means that no module will be marked as ignored.
+2. `ignore_rules.default.ignore_typing`: You don't need to include type hints in the docstrings, though incorrect types will still cause failures.
+3. `ignore_rules.default.ignore_args_and_kwargs`: Documenting `*args` and `**kwargs` parameters in methods and functions isn't required.
+4. `ignore_rules.modules.ignore_prefixes_rules`: deepFlow follows a convention of writing most of the code in private modules and then reimporting the desired objects in the `__init__` module. Even though we are not checking the modules for the docstrings, we would still be ignoring the ones that start with `_` as it is a default ignore rule. Then, most of the code would simply be ignored (elements inside an ignored node are also ignored). Setting no ignore rules for modules means that no module will be marked as ignored.
 #### Flexible Documentation Checking
 
 Sometimes, strict documentation enforcement might not be necessary, but you still want to ensure that the documented nodes are accurate. For example, imagine you've documented a function and later updated its signature. In this case, you'd want doXtrings to alert you about incorrect docstrings but not pester you when docstrings are absent. Achieve this with:
 
 ```toml
-root_dir = "./src/"
+path = "./src/"
 types_to_check = ["function", "method"]
 
-[ignore_filters.default]
+[ignore_rules.default]
 ignore_prefixes_rules = [""]  # Ignores everything
 ```
 
 The key point in this approach is setting an empty string in the `ignore_prefixes_rules`. In Python, all strings start with an empty string, so this will ignore all the nodes. Even ignoring everything, doXtrings will still check functions and methods and report an error if the docstring does not match the signature.
 ### Reference
 
 For all the possible fields in the configuration object, check the documentation reference (`doxtrings.config.DoXtringsConfig`) at the [reference pages](reference/doxtrings/config.md).
```

### Comparing `doxtrings-0.1.1/docs/usage.md` & `doxtrings-0.2.0/docs/usage.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 doxtrings
 ```
 
 If any docstrings are missing or incorrect, the command will display them. Here are some examples:
 
 #### Missing Docstring
 ```
-Docstring error discovered at src/doxtrings/config.py:145 for attribute root_dir
+Docstring error discovered at src/doxtrings/config.py:145 for attribute path
     Location: Reason for missing docstring
 ```
 
-This indicates the absence of a docstring for an attribute called `root_dir`. The specific location is identified as `src/doxtrings/config.py:145`. Most integrated development environments (IDEs) allow you to click on the location to jump to the relevant file.
+This indicates the absence of a docstring for an attribute called `path`. The specific location is identified as `src/doxtrings/config.py:145`. Most integrated development environments (IDEs) allow you to click on the location to jump to the relevant file.
 
 #### Incorrect Return Type
 
 ```
 Docstring error found at src/doxtrings/config.py:279 for function load_config
     At .return_type: Reason for conflicting values; Expected DoXtringsConfig but docstring states obj
 ```
```

### Comparing `doxtrings-0.1.1/mkdocs.yaml` & `doxtrings-0.2.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/pyproject.toml` & `doxtrings-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 """
 testpaths = ["test"]
 
 [tool.isort]
 profile = "black"
 
 [tool.doxtrings]
-root_dir = "./src/doxtrings"
+path = "./src/doxtrings"
 
-[tool.doxtrings.ignore_filters.default]
+[tool.doxtrings.ignore_rules.default]
 ignore_prefixes_rules = ["_"]
 include_prefixes_rules = ["__init__"]
 
-[tool.doxtrings.ignore_filters.variables]
+[tool.doxtrings.ignore_rules.variables]
 ignore_matches = ["logger"]
```

### Comparing `doxtrings-0.1.1/src/doxtrings/cli/scan.py` & `doxtrings-0.2.0/src/doxtrings/cli/scan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The main CLI module, responsible for running all steps of doXtrings scan"""
+
 from argparse import ArgumentParser
 from typing import Optional
 
-from doxtrings.config import set_config
+from doxtrings.config import get_config
 from doxtrings.core.parser.file_parser import DoXtringsAstParser
 from doxtrings.core.report import SimpleReporter
 from doxtrings.core.search import search_files
 
 
 def scan():
     """Runs the full doxtrings scan"""
@@ -16,18 +17,18 @@
 
     arg_parser.add_argument("-c", "--config-file", default=None, required=False)
     args = arg_parser.parse_args()
     _scan(args.config_file)
 
 
 def _scan(config_file: Optional[str]):
-    set_config(config_file=config_file)
-    parser = DoXtringsAstParser()
-    reporter = SimpleReporter()
-    for file in search_files():
+    cfg = get_config(config_file=config_file)
+    parser = DoXtringsAstParser(config_file=config_file)
+    reporter = SimpleReporter(cfg)
+    for file in search_files(cfg):
         for documentable, diffs in parser.parse_file(file):
             reporter.add_documentable_diff(documentable=documentable, diffs=diffs)
     reporter.report()
 
 
 if __name__ == "__main__":
     scan()
```

### Comparing `doxtrings-0.1.1/src/doxtrings/core/parser/file_parser.py` & `doxtrings-0.2.0/src/doxtrings/core/parser/file_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Implements the class responsible for parsing each file into Documentables"""
+
 import ast
 import logging
 from pathlib import Path
 from typing import Dict, Generator, List, Optional, Tuple, Type
 
-from doxtrings.config import DoXtringsConfig, load_config
+from doxtrings.config import DoXtringsConfig, get_config
 from doxtrings.core.parser.node_parser import ParsingContext
 from doxtrings.documentable import Diff, DiffReasons, Documentable
 
 logger = logging.getLogger(__name__)
 
 from doxtrings.core.parser.node_parser import (
     BaseNodeParser,
@@ -21,32 +22,37 @@
 _NodeParserMapping = Dict[Type[ast.AST], List[BaseNodeParser]]
 """Type alias to a mapping of node types to parsers"""
 
 
 class DoXtringsAstParser:
     """Parser class that reads a file and returns a Generator of Documentables"""
 
-    def __init__(self):
-        """Initializes a new DoXtringsAstParser"""
-        self._config = load_config()
-        self._node_parser_mapping = _get_node_to_parser_mapping(self._config)
+    def __init__(self, config_file: Optional[str]):
+        """Initializes the DoXtrings parser
+
+        Args:
+            config_file (Optional[str]): the config file, if given
+        """
+        self._config_file = config_file
 
     def parse_file(
         self, file: Path
     ) -> Generator[Tuple[Documentable, List[Diff]], None, None]:
         """Parses a file into a list of documentables
 
         Args:
             file (Path): path of the file to be parsed
 
         Yields:
             Generator[Tuple[Documentable, List[Diff]], None, None]: generator of tuples
             with documentables and an optional namedtuple with the docstring data.
         """
         logger.info(f"Parsing file {str(file)}")
+        self._config = get_config(self._config_file, file)
+        self._node_parser_mapping = _get_node_to_parser_mapping(self._config)
         self._filename = file.name
         self._filepath = file
         module = _ast_parse(file)
         return self._parse_ast_node(module)
 
     def _parse_ast_node(
         self,
@@ -64,22 +70,27 @@
                     self._filepath, self._filename, context, next_node, ignored_node
                 ),
             )
             # If node is ignored, we mark all the next nodes parsed inside this one as ignored
             if node_data and self._is_documentable_ignored(node_data):
                 ignored_node = True
 
-            if node_data and node_data.documentable_type in self._config.types_to_check:
+            types_to_check = self._config.types_to_check or []
+
+            if node_data and node_data.documentable_type in types_to_check:
                 diffs = parser.get_diffs()
                 logger.debug(f"Found data for node {node}")
                 if len(diffs) and self._should_report_diffs(diffs, ignored_node):
                     logger.info(f"Found diffs for node {node}, yielding")
                     yield node_data, diffs
 
         # Traverse all child nodes
+        assert (
+            self._config.parsing_depth
+        ), "Parsing depth must be set in the configuration"
         if len(context) < self._config.parsing_depth:
             for result in self._traverse_ast(
                 node, context=context, ignored_node=ignored_node
             ):
                 yield result
 
     def _traverse_ast(
@@ -105,15 +116,15 @@
             elif isinstance(value, ast.AST):
                 for result in self._parse_ast_node(
                     value, new_context, ignored_node=ignored_node
                 ):
                     yield result
 
     def _is_documentable_ignored(self, documentable: Documentable) -> bool:
-        ignore_rules = self._config.get_ignore_filters(documentable.documentable_type)
+        ignore_rules = self._config.get_ignore_rules(documentable.documentable_type)
         ignore_matches = (
             [] if ignore_rules.ignore_matches is None else ignore_rules.ignore_matches
         )
         ignore_prefixes_rules = (
             []
             if ignore_rules.ignore_prefixes_rules is None
             else ignore_rules.ignore_prefixes_rules
@@ -145,15 +156,15 @@
 
         # For all other cases, we do want to yield the diffs
         return True
 
 
 def _get_node_to_parser_mapping(config: DoXtringsConfig) -> _NodeParserMapping:
     mapping: _NodeParserMapping = {}
-    parsers = _load_node_parsers()
+    parsers = _load_node_parsers(config)
     for parser in parsers:
         _add_inputs_in_mapping(mapping, parser)
     return mapping
 
 
 def _add_inputs_in_mapping(
     mapping: _NodeParserMapping,
@@ -162,17 +173,22 @@
     inputs = parser.get_input_types()
     for input in inputs:
         if input not in mapping:
             mapping[input] = []
         mapping[input].append(parser)
 
 
-def _load_node_parsers() -> Tuple[BaseNodeParser, ...]:
+def _load_node_parsers(config: DoXtringsConfig) -> Tuple[BaseNodeParser, ...]:
     # TODO make this extensible
-    return (FunctionParser(), ClassParser(), ModuleParser(), VariablesParser())
+    return (
+        FunctionParser(config),
+        ClassParser(config),
+        ModuleParser(config),
+        VariablesParser(config),
+    )
 
 
 def _ast_parse(file: Path) -> ast.Module:
     file_content: str
     with file.open("r") as file_input:
         file_content = file_input.read()
     return ast.parse(file_content, file.name)
```

### Comparing `doxtrings-0.1.1/src/doxtrings/core/parser/node_parser.py` & `doxtrings-0.2.0/src/doxtrings/core/parser/node_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """ Implements classes capable of parsing both the AST nodes and the docstrings into Documentables"""
+
 import ast
 import logging
 from abc import ABC, abstractmethod
 from difflib import SequenceMatcher
 from itertools import zip_longest
 from pathlib import Path
 from typing import Any, List, NamedTuple, Optional, Set, Tuple, Type, Union
 
 import docstring_parser as dp
 
-from doxtrings.config import IgnoreFilters, load_config
+from doxtrings.config import DoXtringsConfig, IgnoreRules
 from doxtrings.documentable import Diff, DiffReasons, Documentable, DocumentableType
 
 logger = logging.getLogger(__name__)
 
 
 class EmptyTuple(NamedTuple):
     """An empty tuple used when there is no relevant data to be stored"""
@@ -43,17 +44,22 @@
 
     _input: ast.AST
     _context: ParsingContext
     _name: str
     _documentable_type: Optional[DocumentableType]
     _lineno: int
 
-    def __init__(self):
-        """Initializes the parser"""
-        self._config = load_config()
+    def __init__(self, config: DoXtringsConfig):
+        """Initializes the parser
+
+        Args:
+            config (DoXtringsConfig): the DoXtrings configuration
+
+        """
+        self._config = config
 
     @classmethod
     @abstractmethod
     def get_input_types(cls) -> Set[Type[ast.AST]]:
         """Returns a set with the AST types this parser can parse from
 
         Returns:
@@ -485,14 +491,18 @@
             type_hint = str(annotation_node.id)
         elif isinstance(annotation_node, ast.Constant):
             type_hint = self._get_constant_string_value(annotation_node.value)
 
         # Recursive methods
         elif isinstance(annotation_node, ast.Subscript):
             type_hint = self._get_subscript_type_hint(annotation_node)
+        elif isinstance(annotation_node, ast.Call):
+            type_hint = self._get_call_type_hint(annotation_node)
+        elif isinstance(annotation_node, ast.keyword):
+            type_hint = self._get_keyword_type_hint(annotation_node)
         elif isinstance(annotation_node, ast.BinOp):
             type_hint = self._get_binop_type_hint(annotation_node)
         elif isinstance(annotation_node, ast.UnaryOp):
             type_hint = self._get_unop_type_hint(annotation_node)
         elif isinstance(annotation_node, ast.Tuple):
             type_hint = self._get_tuple_type_hint(annotation_node)
         elif isinstance(annotation_node, ast.List):
@@ -527,14 +537,28 @@
 
     def _get_subscript_type_hint(self, annotation_node: ast.Subscript):
         outer_value = self._get_type_annotation(annotation_node.value)
         inner_value = self._get_type_annotation(annotation_node.slice)
 
         return f"{outer_value}[{inner_value}]"
 
+    def _get_call_type_hint(self, annotation_node: ast.Call):
+        outer_value = self._get_type_annotation(annotation_node.func)
+        args = [self._get_type_annotation(a) for a in annotation_node.args]
+        keywords = [self._get_keyword_type_hint(k) for k in annotation_node.keywords]
+        inner_values = args + keywords
+        inner_value_string = ", ".join([v for v in inner_values if v is not None])
+
+        return f"{outer_value}({inner_value_string})"
+
+    def _get_keyword_type_hint(self, annotation_node: ast.keyword):
+        return (
+            f"{annotation_node.arg}={self._get_type_annotation(annotation_node.value)}"
+        )
+
     def _get_unop_type_hint(self, annotation_node: ast.UnaryOp):
         operand = self._get_type_annotation(annotation_node.operand)
         if isinstance(annotation_node.op, ast.USub):
             operator = "-"
         elif isinstance(annotation_node.op, ast.UAdd):
             operator = "+"
         elif isinstance(annotation_node.op, ast.Not):
@@ -608,15 +632,15 @@
                 Diff(DiffReasons.NO_DOCSTRING, location=[], code_value=self._code_data)
             ]
 
         if self._docstring_data == self._code_data:
             return []
 
         assert self._documentable_type
-        ignore_config = self._config.get_ignore_filters(self._documentable_type)
+        ignore_config = self._config.get_ignore_rules(self._documentable_type)
         diffs = self._get_arguments_list_diff(ignore_config)
 
         return_type_diff = self._get_type_diff(
             self._code_data.return_type,
             self._docstring_data.return_type,
             ["return_type"],
         )
@@ -628,15 +652,15 @@
                 ignore_config.get_ignore_return()
                 and return_type_diff.reason == DiffReasons.MISSING
             )
             if not should_ignore:
                 diffs.append(return_type_diff)
         return diffs
 
-    def _get_arguments_list_diff(self, ignore_config: IgnoreFilters) -> List[Diff]:
+    def _get_arguments_list_diff(self, ignore_config: IgnoreRules) -> List[Diff]:
         assert self._docstring_data
         if (
             ignore_config.get_ignore_arguments()
             and len(self._docstring_data.arguments) == 0
         ) or (
             ignore_config.get_ignore_arguments()
             and not self._config.fail_ignored_if_incorrect
@@ -704,15 +728,15 @@
         code_value = code_value.replace("\n", " ") if code_value else None
         doc_value = doc_value.replace("\n", " ") if doc_value else None
         # For the code value we strip quotes because those can be omitted in docstring
         # (and its fine)
         no_quotes_code_value = code_value.replace('"', "") if code_value else None
         if code_value != doc_value and no_quotes_code_value != doc_value:
             reason = FunctionParser._get_element_diff_reason(code_value, doc_value)
-            ignore_config = self._config.get_ignore_filters(self._documentable_type)
+            ignore_config = self._config.get_ignore_rules(self._documentable_type)
             should_ignore = (
                 ignore_config.get_ignore_typing()
                 and not self._config.fail_ignored_if_incorrect
             ) or (ignore_config.get_ignore_typing() and reason == DiffReasons.MISSING)
             if not should_ignore:
                 return Diff(
                     reason=reason,
@@ -725,18 +749,19 @@
     def _get_element_diff_reason(code: Any, doc: Any):
         if doc is None:
             return DiffReasons.MISSING
         if code is None:
             return DiffReasons.EXTRA
         return DiffReasons.CONFLICTING_VALUE
 
-    @classmethod
-    def _get_parsing_style(cls) -> dp.DocstringStyle:
-        cfg = load_config()
-        return cls._DOCSTRING_STYLES[cfg.docstring_format]
+    def _get_parsing_style(self) -> dp.DocstringStyle:
+        assert (
+            self._config.docstring_format
+        ), "Docstring format is a required field in the config"
+        return self._DOCSTRING_STYLES[self._config.docstring_format]
 
     @staticmethod
     def _get_docstring_data(docstring: dp.Docstring) -> FunctionData:
         function_args = tuple(
             FunctionArgument(param.arg_name, param.type_name)
             for param in docstring.params
         )
```

### Comparing `doxtrings-0.1.1/src/doxtrings/core/report.py` & `doxtrings-0.2.0/src/doxtrings/core/report.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Implements the classes used to print the reports of the found differences
 found in the source code
 """
+
 import sys
 from abc import ABC, abstractmethod
 from typing import List, NamedTuple, Union
 
-from doxtrings.config import load_config
+from doxtrings.config import DoXtringsConfig
 from doxtrings.core.parser.node_parser import Diff
 from doxtrings.documentable import Documentable
 
 
 class ReportItem(NamedTuple):
     """A NamedTuple containing the relevant report data for a single documentable"""
 
@@ -19,17 +20,21 @@
     diffs: List[Diff]
     """The documentable's list of differences"""
 
 
 class BaseReporter(ABC):
     """Base reporter class"""
 
-    def __init__(self):
-        """Initializes the base reporter with an empty list of report items"""
-        self._config = load_config()
+    def __init__(self, config: DoXtringsConfig):
+        """Initializes the base reporter with an empty list of report items
+
+        Args:
+            config (DoXtringsConfig): the DoXtrings configuration
+        """
+        self._config = config
         self.report_items: List[ReportItem] = []
 
     def add_documentable_diff(self, documentable: Documentable, diffs: List[Diff]):
         """
         Adds a list of diffs to a documentable. The provided `diffs` argument is filtered
         according to configuration rules before being linked to the documentable in a ReportItem.
```

### Comparing `doxtrings-0.1.1/src/doxtrings/core/search.py` & `doxtrings-0.2.0/src/doxtrings/core/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Implements the functions used to search a directory for the files to be parsed by doXtrings"""
+
 import logging
 from os import walk
 from pathlib import Path
-from typing import Generator, List
+from typing import Generator, List, Optional
 
-from doxtrings.config import load_config
+from doxtrings.config import DoXtringsConfig
 
 logger = logging.getLogger(__name__)
 
 
-def search_files() -> Generator[Path, None, None]:
+def search_files(config: DoXtringsConfig) -> Generator[Path, None, None]:
     """Runs through the directory specified in the config and yields file paths to be parsed.
 
+    Args:
+        config (DoXtringsConfig): the DoXtrings configuration
+
     Yields:
         Generator[Path, None, None]: the file paths to be parsed
     """
-    config = load_config()
-    for dirpath, subdirs, filenames in walk(config.root_dir):
+    for dirpath, subdirs, filenames in walk(config.path):
         logger.debug(f"Searching files at {dirpath}")
         for filename in filenames:
             if _should_include_file(
                 filename, config.exclude_files, config.include_file_extensions
             ):
                 file_path = Path(dirpath) / filename
                 logger.debug(f"Yielding file {str(file_path)}")
@@ -32,30 +35,38 @@
             for subdir in subdirs
             if _should_include_dir(subdir, config.exclude_files)
         ]
         logger.debug(f"Looking into subdirs {subdirs}")
 
 
 def _should_include_file(
-    filename: str, exclude_list: List[str], allowed_extensions: List[str]
+    filename: str,
+    exclude_list: Optional[List[str]],
+    allowed_extensions: Optional[List[str]],
 ):
+    if exclude_list is None:
+        exclude_list = []
+    if allowed_extensions is None:
+        allowed_extensions = []
     suffix_match = _match_suffix(filename, allowed_extensions)
     if not suffix_match:
         logger.info(
             f"File {filename} excluded because extension does not match any of: {allowed_extensions}"
         )
     excluded = filename in exclude_list
     if excluded:
         logger.info(
             f"File {filename} excluded because found match in exclude list: {exclude_list}"
         )
     return suffix_match and not excluded
 
 
-def _should_include_dir(dirname: str, exclude_list: List[str]):
+def _should_include_dir(dirname: str, exclude_list: Optional[List[str]]):
+    if exclude_list is None:
+        exclude_list = []
     excluded = dirname in [excluded.strip("/") for excluded in exclude_list]
     if excluded:
         logger.info(
             f"Directory {dirname} excluded because found match in exclude list: {exclude_list}"
         )
     return not excluded
```

### Comparing `doxtrings-0.1.1/src/doxtrings/documentable.py` & `doxtrings-0.2.0/src/doxtrings/documentable.py`

 * *Files identical despite different names*

### Comparing `doxtrings-0.1.1/PKG-INFO` & `doxtrings-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doxtrings
-Version: 0.1.1
+Version: 0.2.0
 Summary: a package that can ensure your docstrings are correct
 Author-email: Lucas Pereira <pereira.lucas@bcg.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: tomli==2.*
 Requires-Dist: docstring-parser==0.15
 Requires-Dist: bump2version==1.0.1 ; extra == "ci"
```

