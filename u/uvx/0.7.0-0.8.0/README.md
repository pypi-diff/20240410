# Comparing `tmp/uvx-0.7.0.tar.gz` & `tmp/uvx-0.8.0.tar.gz`

## Comparing `uvx-0.7.0.tar` & `uvx-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 uvx-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_constants.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_maybe.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_python.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_symlinks.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/cli.py
--rw-r--r--   0        0        0    15071 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/core.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.7.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.7.0/README.md
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 uvx-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 uvx-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 uvx-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_cli_support.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_constants.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_maybe.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_python.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_symlinks.py
+-rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/cli.py
+-rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/core.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.8.0/README.md
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 uvx-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 uvx-0.8.0/PKG-INFO
```

### Comparing `uvx-0.7.0/CHANGELOG.md` & `uvx-0.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.8.0 (2024-04-10)
+
+### Feature
+
+* Added `--verbose` flag to global state (+ used by --verbose) ([`8c20be4`](https://github.com/robinvandernoord/uvx/commit/8c20be4c82a8ecd8abe9d7e8615c3da28304c8b4))
+
+### Fix
+
+* Work in progress on `self-update` ([`56dec48`](https://github.com/robinvandernoord/uvx/commit/56dec48a0abb7b32efab5e4e10a034e383b36eb9))
+
 ## v0.7.0 (2024-04-10)
 
 ### Feature
 
 * `uvx upgrade-all` ([`5edc7af`](https://github.com/robinvandernoord/uvx/commit/5edc7afeda4bb544b346f962a730f66c6b92dbf8))
 
 ### Fix
```

### Comparing `uvx-0.7.0/src/uvx/_python.py` & `uvx-0.8.0/src/uvx/_python.py`

 * *Files identical despite different names*

### Comparing `uvx-0.7.0/src/uvx/_symlinks.py` & `uvx-0.8.0/src/uvx/_symlinks.py`

 * *Files identical despite different names*

### Comparing `uvx-0.7.0/src/uvx/cli.py` & `uvx-0.8.0/src/uvx/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This file builds the Typer cli."""
 
+import functools
 import os
 import subprocess  # nosec
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Annotated
 
@@ -11,30 +12,32 @@
 import typer
 from result import Err, Ok, Result
 from typer import Context
 
 from uvx._constants import BIN_DIR
 
 from .__about__ import __version__
+from ._cli_support import State
 from ._maybe import Maybe
-from ._python import _python_in_venv, _uv
+from ._python import _python_in_venv, _uv, _pip
 from .core import (
     as_virtualenv,
     format_bools,
     inject_packages,
     install_package,
     list_packages,
     reinstall_package,
     run_command,
     uninstall_package,
     upgrade_package,
 )
 from .metadata import Metadata
 
 app = typer.Typer()
+state = State()
 
 
 def output(result: Result[str, Exception]) -> None:
     """Output positive (ok) result to stdout and error result to stderr."""
     match result:
         case Ok(msg):
             rich.print(msg)
@@ -121,35 +124,39 @@
         inject_packages(
             into,
             set(package_specs),
         )
     )
 
 
-# todo:
-# self-upgrade (uv and uvx)
-# upgrade-all
-
 @app.command()
 def upgrade_all(
     force: Annotated[bool, typer.Option("-f", "--force", help="Ignore previous version constraint")] = False,
     skip_injected: Annotated[
         bool, typer.Option("--skip-injected", help="Don't also upgrade injected packages")
     ] = False,
     no_cache: Annotated[bool, typer.Option("--no-cache", help="Run without `uv` cache")] = False,
 ):
     """Upgrade all uvx-installed packages."""
+    for venv_name, _ in list_packages():
+        upgrade(venv_name, force=force, skip_injected=skip_injected, no_cache=no_cache)
 
-    for (venv_name, _) in list_packages():
-        upgrade(
-            venv_name,
-            force=force,
-            skip_injected=skip_injected,
-            no_cache=no_cache
-        )
+
+@app.command()
+def self_update(
+    with_uv: Annotated[bool, typer.Option("--with-uv/--without-uv", '-w/-W')] = True,
+):
+    # if in venv and uv available -> upgrade via uv
+    # else: upgrade via pip
+    if os.getenv("VIRTUAL_ENV"):
+        print(_uv)
+    else:
+        print(_pip)
+
+    print(f'self update {with_uv = }')
 
 
 # list
 def _list_short(name: str, metadata: Maybe[Metadata]):
     rich.print("-", name, metadata.map_or("[red]?[/red]", lambda md: md.installed_version))
 
 
@@ -198,14 +205,16 @@
         )
     )
 
 
 @app.command(name="list")
 def list_venvs(short: bool = False, verbose: bool = False, json: bool = False):
     """List packages and apps installed with uvx."""
+    verbose = verbose or state.verbose
+
     if json:
         return _list_venvs_json()
 
     for name, metadata in list_packages():
         if short:
             _list_short(name, metadata)
         else:
@@ -267,34 +276,43 @@
         or --show-completion to see what would be installed.
     """
     rich.print("Use 'uvx --install-completion' to install the autocomplete script to your '.bashrc' file.")
 
 
 def version_callback():
     """Show the current versions when running with --version."""
-    rich.print("uvx", __version__)
-    run_command(str(_uv), "--version", printfn=rich.print)
-    rich.print("Python", sys.version.split(" ")[0])
+    if state.verbose:
+        rich.print("uvx", __version__, sys.argv[0])
+        run_command(str(_uv), "--version", printfn=functools.partial(rich.print, end=" "))
+        rich.print(str(_uv))
+        rich.print("Python", sys.version.split(" ")[0], sys.executable)
+    else:
+        rich.print("uvx", __version__)
+        run_command(str(_uv), "--version", printfn=rich.print)
+        rich.print("Python", sys.version.split(" ")[0])
 
 
 @app.callback(invoke_without_command=True, no_args_is_help=True)
 def main(
     ctx: typer.Context,
+    verbose: bool = False,
     # stops the program:
     version: bool = False,
 ) -> None:  # noqa
     """
     This callback will run before every command, setting the right global flags.
 
     Args:
         ctx: context to determine if a subcommand is passed, etc
-
+        verbose: show more info in supported subcommands?
         version: display current version?
 
     """
+    state.verbose = verbose
+
     if version:
         version_callback()
     elif not ctx.invoked_subcommand:
         rich.print("[yellow]Missing subcommand. Try `uvx --help` for more info.[/yellow]")
     # else: just continue
```

### Comparing `uvx-0.7.0/src/uvx/core.py` & `uvx-0.8.0/src/uvx/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,16 +330,18 @@
         meta.requested_version = version
         new_version = meta.installed_version = get_package_version(meta.name, venv)
         store_metadata(meta, venv)
 
     if old_version == new_version:
         msg = f"🌟 '{package_name}' is already up to date at version {new_version}!"
         if meta.requested_version:
-            msg += (f"\n💡 This package was installed with a version constraint ({meta.requested_version}). "
-                    f"If you want to ignore this constraint, use `uvx upgrade --force {package_name}`.")
+            msg += (
+                f"\n💡 This package was installed with a version constraint ({meta.requested_version}). "
+                f"If you want to ignore this constraint, use `uvx upgrade --force {package_name}`."
+            )
 
     else:
         msg = f"🚀 Successfully updated '{package_name}' from version {old_version} to version {new_version}!"
 
     return Ok(msg)
```

### Comparing `uvx-0.7.0/src/uvx/metadata.py` & `uvx-0.8.0/src/uvx/metadata.py`

 * *Files identical despite different names*

### Comparing `uvx-0.7.0/LICENSE.txt` & `uvx-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uvx-0.7.0/README.md` & `uvx-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `uvx-0.7.0/pyproject.toml` & `uvx-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-0.7.0/PKG-INFO` & `uvx-0.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvx
-Version: 0.7.0
+Version: 0.8.0
 Summary: uvx: pipx for uv
 Project-URL: Documentation, https://github.com/robinvandernoord/uvx#readme
 Project-URL: Issues, https://github.com/robinvandernoord/uvx/issues
 Project-URL: Source, https://github.com/robinvandernoord/uvx
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

