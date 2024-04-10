# Comparing `tmp/colcon-meson-0.4.3.tar.gz` & `tmp/colcon-meson-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colcon-meson-0.4.3.tar", last modified: Sat Apr  6 17:55:29 2024, max compression
+gzip compressed data, was "colcon-meson-0.4.4.tar", last modified: Wed Apr 10 17:06:04 2024, max compression
```

## Comparing `colcon-meson-0.4.3.tar` & `colcon-meson-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/
--rw-rw-r--   0 christian  (1000) christian  (1000)    11357 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/LICENSE
--rw-rw-r--   0 christian  (1000) christian  (1000)     1073 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)      630 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/README.md
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-06 17:55:29.228943 colcon-meson-0.4.3/colcon_meson/
--rw-rw-r--   0 christian  (1000) christian  (1000)        0 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/colcon_meson/__init__.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     8340 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/colcon_meson/build.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     3928 2024-04-06 17:52:20.000000 colcon-meson-0.4.3/colcon_meson/identification.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/colcon_meson.egg-info/
--rw-rw-r--   0 christian  (1000) christian  (1000)     1073 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)      332 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/SOURCES.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        1 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/dependency_links.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)      217 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/entry_points.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)       54 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/requires.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)       13 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/top_level.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)      862 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/setup.cfg
--rw-rw-r--   0 christian  (1000) christian  (1000)       38 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/setup.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/
+-rw-rw-r--   0 christian  (1000) christian  (1000)    11357 2024-03-31 16:27:09.000000 colcon-meson-0.4.4/LICENSE
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1094 2024-04-10 17:06:04.469612 colcon-meson-0.4.4/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      630 2024-03-31 16:27:09.000000 colcon-meson-0.4.4/README.md
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/colcon_meson/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        0 2024-03-31 16:27:09.000000 colcon-meson-0.4.4/colcon_meson/__init__.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    10717 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/colcon_meson/build.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4737 2024-04-10 17:04:02.000000 colcon-meson-0.4.4/colcon_meson/identification.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/colcon_meson.egg-info/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1094 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      436 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/SOURCES.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        1 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/dependency_links.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)      217 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/entry_points.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)      280 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/requires.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)       13 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/top_level.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1278 2024-04-10 17:06:04.469612 colcon-meson-0.4.4/setup.cfg
+-rw-rw-r--   0 christian  (1000) christian  (1000)      121 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/setup.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/test/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1339 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/test/test_copyright_license.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1899 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/test/test_flake8.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      549 2024-04-10 17:04:02.000000 colcon-meson-0.4.4/test/test_identification.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1929 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/test/test_spell_check.py
```

### Comparing `colcon-meson-0.4.3/LICENSE` & `colcon-meson-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.3/PKG-INFO` & `colcon-meson-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: colcon-meson
-Version: 0.4.3
+Version: 0.4.4
 Summary: Extension for colcon to support Meson packages.
 Author: Christian Rauch
 Author-email: Rauch.Christian@gmx.de
 Maintainer: Christian Rauch
 Maintainer-email: Rauch.Christian@gmx.de
 License: Apache License, Version 2.0
 Project-URL: GitHub, https://github.com/colcon/colcon-meson
 Keywords: colcon
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # colcon-meson
 
 A colcon extension for building [Meson](https://mesonbuild.com) packages.
 
 Install from the Python Package Index via:
```

### Comparing `colcon-meson-0.4.3/README.md` & `colcon-meson-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.3/colcon_meson/build.py` & `colcon-meson-0.4.4/colcon_meson/build.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,113 @@
+# Copyright 2024 Christian Rauch
+# Licensed under the Apache License, Version 2.0
+
+from argparse import ArgumentParser, Namespace
+import json
 import os
 from pathlib import Path
 import shutil
-import json
-
-from mesonbuild import coredata
-from mesonbuild.mesonmain import CommandLineParser
 
+# colcon
 from colcon_core.environment import create_environment_scripts
 from colcon_core.logging import colcon_logger
 from colcon_core.shell import get_command_environment
 from colcon_core.task import run
 from colcon_core.task import TaskExtensionPoint
+# meson
+from mesonbuild import coredata
+from mesonbuild.mesonmain import CommandLineParser
 
 logger = colcon_logger.getChild(__name__)
 
 
 def cfg_changed(old, new):
+    """Compare two configurations and return true if they are equal.
+
+    Args:
+        old (dict): old configuration
+        new (dict): new configuration
+
+    Returns:
+        bool: true if configurations are equal and false otherwise
+    """
     for p in old.keys() & new.keys():
         n = new[p]
         # convert string representations of boolen values
         if type(old[p]) is bool and type(n) is str:
             n = bool(n.lower() == "true")
         if n != old[p]:
             logger.debug("option '{}' changed from '{}' to '{}'".format(p, old[p], n))
             return True
     return False
 
 
 def cfg_diff(old, new):
+    """Compare two configurations and return the change.
+
+    Args:
+        old (dict): old configuration
+        new (dict): new configuration
+
+    Returns:
+        (dict, dict): tuple with key-value pairs that were added and remove
+                      between the old and new configuration
+    """
     # get changes between old and new configuration
     k_removed = set(old.keys()) - set(new.keys())
     k_added = set(new.keys()) - set(old.keys())
     d_removed = {k: old[k] for k in k_removed}
     d_added = {k: new[k] for k in k_added}
     return d_added, d_removed
 
 
 def format_args(args):
+    """Convert Meson command line arguments into key-value pairs.
+
+    Args:
+        args: Meson command line arguments
+
+    Returns:
+        dict: converted arguments as key-value pairs
+    """
     return {arg.name: args.cmd_line_options[arg] for arg in args.cmd_line_options}
 
 
 class MesonBuildTask(TaskExtensionPoint):
+    """Task to build a Meson project."""
+
     def __init__(self):
+        """Initialise the build task by discovering meson and setting up the parser."""
         super().__init__()
 
         self.meson_path = shutil.which("meson")
         self.parser_setup = CommandLineParser().subparsers.choices["setup"]
 
-    def add_arguments(self, *, parser):
-        parser.add_argument('--meson-args',
-            nargs='*', metavar='*', type=str.lstrip, default=list(),
-            help="Pass 'setup' arguments to Meson projects.")
+    def add_arguments(self, *, parser: ArgumentParser):
+        """Add new arguments to the colcon build argument parser.
 
-    def get_default_args(self, args):
-        margs = list()
+        Args:
+            parser (ArgumentParser): argument parser
+        """
+        parser.add_argument('--meson-args',
+                            nargs='*', metavar='*',
+                            type=str.lstrip, default=[],
+                            help="Pass 'setup' arguments to Meson projects.",
+                            )
+
+    def get_default_args(self, args: Namespace) -> list[str]:
+        """Get default Meson arguments.
+
+        Args:
+            args (Namespace): parse arguments from an ArgumentParser
+
+        Returns:
+            list: list of command line arguments for meson
+        """
+        margs = []
 
         # meson installs by default to architecture specific subdirectories,
         # e.g. "lib/x86_64-linux-gnu", but the LibraryPathEnvironment hook
         # only searches within the fist lib level
         margs += ["--libdir=lib"]
 
         margs += ["--prefix=" + args.install_base]
@@ -67,29 +117,58 @@
 
         # positional arguments for 'builddir' and 'sourcedir'
         margs += [args.build_base]
         margs += [args.path]
 
         return margs
 
-    def meson_parse_cmdline(self, cmdline):
+    def meson_parse_cmdline(self, cmdline: list[str]) -> Namespace:
+        """Parse command line arguments with the Meson arg parser.
+
+        Args:
+            cmdline (list): command line arguments
+
+        Returns:
+            Namespace: parse args
+        """
         args = self.parser_setup.parse_args(cmdline)
         coredata.parse_cmd_line_options(args)
         return args
 
-    def meson_format_cmdline(self, cmdline):
+    def meson_format_cmdline(self, cmdline: list[str]):
+        """Convert Meson args from command line.
+
+        Args:
+            cmdline (list): command line arguments
+
+        Returns:
+            dict: converted key-value pairs
+        """
         return format_args(self.meson_parse_cmdline(cmdline))
 
-    def meson_format_cmdline_file(self, builddir):
+    def meson_format_cmdline_file(self, builddir: str):
+        """Convert Meson args from command line arguments stored in the build directory.
+
+        Args:
+            builddir (str): path to the build directory
+
+        Returns:
+            dict: converted key-value pairs
+        """
         args = self.meson_parse_cmdline([])
         coredata.read_cmd_line_file(builddir, args)
         return format_args(args)
 
     async def build(self, *, additional_hooks=None, skip_hook_creation=False,
                     environment_callback=None, additional_targets=None):
+        """Full build pipeline for a Meson project.
+
+        Returns:
+            int: return code
+        """
         args = self.context.args
 
         try:
             env = await get_command_environment('build', args.build_base, self.context.dependencies)
         except RuntimeError as e:
             logger.error(str(e))
             return 1
@@ -140,25 +219,25 @@
 
             # restore default values if argument was removed
             for arg in removed.keys():
                 if arg in defcfg and removed[arg] != defcfg[arg]:
                     newcfg[arg] = defcfg[arg]
 
             # parse old configuration from meson cache
-            assert(configfile.exists())
+            assert configfile.exists()
             with open(configfile, 'r') as f:
                 mesoncfg = {arg["name"]: arg["value"] for arg in json.load(f)}
 
             # check if command line arguments would change the current meson settings
             config_changed = cfg_changed(mesoncfg, newcfg)
 
         if not run_init_setup and not config_changed:
             return
 
-        cmd = list()
+        cmd = []
         cmd += [self.meson_path]
         cmd += ["setup"]
         cmd.extend(marg_def)
         if config_changed:
             logger.info("reconfiguring '{}' because configuration changed".format(self.context.pkg.name))
             cmd += ["--reconfigure"]
         if args.meson_args:
@@ -168,15 +247,15 @@
         if completed.returncode:
             logger.error("\n"+completed.stdout.decode('utf-8'))
         return completed.returncode
 
     async def _build(self, args, env, *, additional_targets=None):
         self.progress('build')
 
-        cmd = list()
+        cmd = []
         cmd += [self.meson_path]
         cmd += ["compile"]
 
         # append content from the 'MAKEFLAGS' environment variable
         makeflags = env.get("MAKEFLAGS")
         if makeflags:
             cmd.extend(makeflags.split())
@@ -189,17 +268,17 @@
     async def _install(self, args, env):
         self.progress('install')
 
         mesontargetfile = Path(args.build_base) / "meson-info" / "intro-targets.json"
         lastinstalltargetfile = Path(args.build_base) / "last_install_targets.json"
 
         # get current install targets
-        assert(mesontargetfile.exists())
+        assert mesontargetfile.exists()
         with open(mesontargetfile, 'r') as f:
-            install_targets = {target["name"]:target["install_filename"] for target in json.load(f) if target["installed"]}
+            install_targets = {target["name"]: target["install_filename"] for target in json.load(f) if target["installed"]}
 
         if not install_targets:
             logger.error("no install targets")
 
         # remove files of removed install targets
         if lastinstalltargetfile.exists():
             with open(lastinstalltargetfile, 'r') as f:
@@ -216,27 +295,31 @@
                         os.remove(path)
                     elif os.path.isdir(path):
                         shutil.rmtree(path)
 
         with open(lastinstalltargetfile, 'w') as f:
             json.dump(install_targets, f)
 
-        cmd = list()
+        cmd = []
         cmd += [self.meson_path]
         cmd += ["install"]
 
         completed = await run(self.context, cmd, cwd=args.build_base, env=env, capture_output="stdout")
         if completed.returncode:
             logger.error("\n"+completed.stdout.decode('utf-8'))
         return completed.returncode
 
 
 class RosMesonBuildTask(TaskExtensionPoint):
-    def __init__(self):
-        super().__init__()
+    """Task to build a Meson project."""
 
     async def build(self):
+        """Full build pipeline for a Meson project with a package.xml.
+
+        Returns:
+            int: return code
+        """
         meson_extension = MesonBuildTask()
         meson_extension.set_context(context=self.context)
         rc = await meson_extension.build()
         if rc:
             return rc
```

### Comparing `colcon-meson-0.4.3/colcon_meson/identification.py` & `colcon-meson-0.4.4/colcon_meson/identification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,78 @@
+# Copyright 2024 Christian Rauch
+# Licensed under the Apache License, Version 2.0
+
 import os
 import typing
 
+# colcon
+from colcon_core.logging import colcon_logger
+from colcon_core.package_descriptor import PackageDescriptor
+from colcon_core.package_identification import PackageIdentificationExtensionPoint
+# meson
 from mesonbuild import environment
 from mesonbuild import mesonlib
-from mesonbuild.interpreterbase.interpreterbase import InterpreterBase
-from mesonbuild.interpreterbase.baseobjects import *
 from mesonbuild.interpreter import primitives
-
-from colcon_core.logging import colcon_logger
-from colcon_core.package_identification import PackageIdentificationExtensionPoint
+from mesonbuild.interpreterbase.baseobjects import InterpreterObject, mparser
+from mesonbuild.interpreterbase.interpreterbase import InterpreterBase
 
 logger = colcon_logger.getChild(__name__)
 
 
 class CustomInterpreter(InterpreterBase):
+    """A custom interpreter to parse metadata for Meson projects."""
+
     def __init__(self, source_root: str, subdir: str, subproject: str):
+        """Initialise the interpreter and a data structure for metadata."""
         super().__init__(source_root, subdir, subproject)
 
         self.holder_map.update({
             list: primitives.ArrayHolder,
             dict: primitives.DictHolder,
             int: primitives.IntegerHolder,
             bool: primitives.BooleanHolder,
             str: primitives.StringHolder,
         })
 
         self.environment = environment
 
-        self.data = dict()
+        self.data = {}
         self.data["dependencies"] = set()
 
     def evaluate_statement(self, cur: mparser.BaseNode) -> typing.Optional[InterpreterObject]:
+        """Evaluate the statements in the Meson project file.
+
+        Args:
+            cur (mparser.BaseNode): a node in the project file
+
+        Returns:
+            typing.Optional[InterpreterObject]:
+        """
         if isinstance(cur, mparser.FunctionNode):
-            return self.function_call(cur)
+            return self._function_call(cur)
         elif isinstance(cur, mparser.AssignmentNode):
-            self.assignment(cur)
+            self._assignment(cur)
         elif isinstance(cur, mparser.StringNode):
             return self._holderify(cur.value)
         elif isinstance(cur, mparser.ArrayNode):
-            return self.evaluate_arraystatement(cur)
+            return self._evaluate_arraystatement(cur)
         return None
 
-    def function_call(self, node: mparser.FunctionNode) -> typing.Optional[InterpreterObject]:
+    def _function_call(self, node: mparser.FunctionNode) -> typing.Optional[InterpreterObject]:
         node_func_name = f"{type(node.func_name).__module__}.{type(node.func_name).__qualname__}"
-        if node_func_name == "str":
+        if node_func_name == "builtins.str":
             # meson <= 1.2
             func_name = node.func_name
         elif node_func_name == "mesonbuild.mparser.IdNode":
             # meson >= 1.3
             func_name = node.func_name.value
         else:
             raise AttributeError("Cannot determine meson project name.")
 
-        assert type(func_name) == str
+        assert type(func_name) is str
 
         reduced_pos = [self.evaluate_statement(arg) for arg in node.args.arguments]
         reduced_pos = list(filter(None, reduced_pos))
         args = self._unholder_args(reduced_pos, {})[0]
 
         if func_name == "project":
             self.data["name"] = args[0]
@@ -66,46 +82,55 @@
             subpath = os.path.join(self.source_root, args[0])
             parser = CustomInterpreter(subpath, "", "")
             subdata = parser.parse()
             for k in subdata.keys():
                 self.data[k].update(subdata[k])
         return None
 
-    def assignment(self, node: mparser.AssignmentNode) -> None:
+    def _assignment(self, node: mparser.AssignmentNode) -> None:
         self.evaluate_statement(node.value)
         return None
 
-    def evaluate_arraystatement(self, cur: mparser.ArrayNode) -> InterpreterObject:
+    def _evaluate_arraystatement(self, cur: mparser.ArrayNode) -> InterpreterObject:
         arguments = [self.evaluate_statement(arg) for arg in cur.args.arguments]
         arguments = list(filter(None, arguments))
         return self._holderify(self._unholder_args(arguments, {})[0])
 
     def parse(self) -> dict:
+        """Run the interpreter on a Meson project file.
+
+        Returns:
+            dict: extracted metadata
+        """
         try:
             self.load_root_meson_file()
         except mesonlib.MesonException:
-            return dict()
+            return {}
 
         self.evaluate_codeblock(self.ast)
         return self.data
 
 
 class MesonPackageIdentification(PackageIdentificationExtensionPoint):
-    def __init__(self):
-        super().__init__()
+    """Meson package identification."""
+
+    def identify(self, desc: PackageDescriptor):
+        """Identify a Meson project for colcon.
 
-    def identify(self, metadata):
-        parser = CustomInterpreter(metadata.path, "", "")
+        Args:
+            desc (PackageDescriptor): package description that will be updated
+        """
+        parser = CustomInterpreter(desc.path, "", "")
         data = parser.parse()
 
         if not data:
             return
 
-        metadata.type = 'meson'
+        desc.type = 'meson'
 
-        if metadata.name is None:
-            metadata.name = data["name"]
+        if desc.name is None:
+            desc.name = data["name"]
 
-        logger.info("'%s' dependencies: %s", metadata.name, data['dependencies'])
+        logger.info("'%s' dependencies: %s", desc.name, data['dependencies'])
 
-        metadata.dependencies['build'].update(data['dependencies'])
-        metadata.dependencies['run'].update(data['dependencies'])
+        desc.dependencies['build'].update(data['dependencies'])
+        desc.dependencies['run'].update(data['dependencies'])
```

### Comparing `colcon-meson-0.4.3/colcon_meson.egg-info/PKG-INFO` & `colcon-meson-0.4.4/colcon_meson.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: colcon-meson
-Version: 0.4.3
+Version: 0.4.4
 Summary: Extension for colcon to support Meson packages.
 Author: Christian Rauch
 Author-email: Rauch.Christian@gmx.de
 Maintainer: Christian Rauch
 Maintainer-email: Rauch.Christian@gmx.de
 License: Apache License, Version 2.0
 Project-URL: GitHub, https://github.com/colcon/colcon-meson
 Keywords: colcon
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # colcon-meson
 
 A colcon extension for building [Meson](https://mesonbuild.com) packages.
 
 Install from the Python Package Index via:
```

### Comparing `colcon-meson-0.4.3/setup.cfg` & `colcon-meson-0.4.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = colcon-meson
-version = 0.4.3
+version = 0.4.4
 project_urls = 
 	GitHub = https://github.com/colcon/colcon-meson
 author = Christian Rauch
 author_email = Rauch.Christian@gmx.de
 maintainer = Christian Rauch
 maintainer_email = Rauch.Christian@gmx.de
 license = Apache License, Version 2.0
@@ -17,18 +17,47 @@
 python_requires = >=3.6
 install_requires = 
 	colcon-core >= 0.10.0
 	colcon-library-path
 	meson >= 0.60.0
 packages = find:
 
+[options.extras_require]
+test = 
+	flake8>=3.6.0,<6
+	flake8-blind-except
+	flake8-builtins
+	flake8-class-newline
+	flake8-comprehensions
+	flake8-deprecated
+	flake8-docstrings
+	flake8-import-order
+	flake8-quotes
+	pep8-naming
+	pylint
+	pytest
+	pytest-cov
+	scspell3k>=2.2
+
+[tool:pytest]
+junit_suite_name = colcon-meson
+markers = 
+	flake8
+	linter
+
 [options.entry_points]
 colcon_core.package_identification = 
 	meson = colcon_meson.identification:MesonPackageIdentification
 colcon_core.task.build = 
 	meson = colcon_meson.build:MesonBuildTask
 	ros.meson = colcon_meson.build:RosMesonBuildTask
 
+[flake8]
+import-order-style = google
+
+[coverage:run]
+source = colcon_meson
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

