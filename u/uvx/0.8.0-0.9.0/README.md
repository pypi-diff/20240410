# Comparing `tmp/uvx-0.8.0.tar.gz` & `tmp/uvx-0.9.0.tar.gz`

## Comparing `uvx-0.8.0.tar` & `uvx-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 uvx-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_cli_support.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_constants.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_maybe.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_python.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/_symlinks.py
--rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/cli.py
--rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/core.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.8.0/src/uvx/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.8.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.8.0/README.md
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 uvx-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 uvx-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 uvx-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/_cli_support.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/_constants.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/_maybe.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/_python.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/_symlinks.py
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/cli.py
+-rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/core.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.9.0/src/uvx/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.9.0/README.md
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 uvx-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 uvx-0.9.0/PKG-INFO
```

### Comparing `uvx-0.8.0/CHANGELOG.md` & `uvx-0.9.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.9.0 (2024-04-10)
+
+### Feature
+
+* Added `uvx self-update` ([`986c7b5`](https://github.com/robinvandernoord/uvx/commit/986c7b55fda215ff877e256e5c88b2f4c3882245))
+
 ## v0.8.0 (2024-04-10)
 
 ### Feature
 
 * Added `--verbose` flag to global state (+ used by --verbose) ([`8c20be4`](https://github.com/robinvandernoord/uvx/commit/8c20be4c82a8ecd8abe9d7e8615c3da28304c8b4))
 
 ### Fix
```

### Comparing `uvx-0.8.0/src/uvx/_python.py` & `uvx-0.9.0/src/uvx/_python.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import sys
 import textwrap
+import typing
 from pathlib import Path
 
 import plumbum  # type: ignore
 from plumbum.cmd import grep  # type: ignore
+from plumbum.commands.base import BoundCommand  # type: ignore
 from plumbum.machines.local import LocalCommand  # type: ignore
 from uv import find_uv_bin
 
 _python = plumbum.local[sys.executable]
 _pip = _python["-m", "pip"]
 _uv = plumbum.local[find_uv_bin()]
 
@@ -50,15 +52,34 @@
 
 def get_python_executable(venv: Path):
     """Get the Python executable for a venv (used to determine the version)."""
     executable = venv / "bin" / "python"  # DON'T use _python_in_venv because we want to resolve the symlink:
     return str(executable.resolve())  # /usr/bin/python3.xx
 
 
+T = typing.TypeVar("T")
+
+RAISE = object()  # special sentry object
+
+
+def _get_package_version(package: str, pip_list: BoundCommand, default: T) -> str | T:
+    try:
+        regex = f"^({package}==|{package} @)"
+        line: str = (pip_list | grep["-E", regex])().strip()
+        return (line.split("@")[-1] if "@" in line else line.split("==")[-1]).strip()
+    except Exception as e:
+        if default is RAISE:
+            raise e
+
+        return default
+
+
 def get_package_version(package: str, venv: Path) -> str:
     """Get the currently installed version of a specific package."""
     # assumes `with virtualenv(venv)` block executing this function
     uv = _uv_in_venv(venv)
 
-    regex = f"^({package}==|{package} @)"
-    line: str = (uv["pip", "freeze"] | grep["-E", regex])().strip()
-    return (line.split("@")[-1] if "@" in line else line.split("==")[-1]).strip()
+    return _get_package_version(
+        package,
+        uv["pip", "freeze"],
+        default="",
+    )
```

### Comparing `uvx-0.8.0/src/uvx/_symlinks.py` & `uvx-0.9.0/src/uvx/_symlinks.py`

 * *Files identical despite different names*

### Comparing `uvx-0.8.0/src/uvx/cli.py` & `uvx-0.9.0/src/uvx/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 import os
 import subprocess  # nosec
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Annotated
 
+import plumbum as pb  # type: ignore
 import rich
 import typer
+from plumbum import local
+from plumbum.commands.base import BoundCommand  # type: ignore
 from result import Err, Ok, Result
 from typer import Context
 
 from uvx._constants import BIN_DIR
 
 from .__about__ import __version__
 from ._cli_support import State
 from ._maybe import Maybe
-from ._python import _python_in_venv, _uv, _pip
+from ._python import _get_package_version, _pip, _python_in_venv, _uv
 from .core import (
     as_virtualenv,
     format_bools,
     inject_packages,
     install_package,
     list_packages,
     reinstall_package,
@@ -137,26 +140,76 @@
     no_cache: Annotated[bool, typer.Option("--no-cache", help="Run without `uv` cache")] = False,
 ):
     """Upgrade all uvx-installed packages."""
     for venv_name, _ in list_packages():
         upgrade(venv_name, force=force, skip_injected=skip_injected, no_cache=no_cache)
 
 
+def _self_update_via_cmd(pip_ish: BoundCommand, with_uv: bool):
+    old = {}
+    new = {}
+
+    old["uv"] = _get_package_version("uv", pip_ish["freeze"], default="unknown")
+
+    old["uvx"] = _get_package_version("uvx", pip_ish["freeze"], default="unknown")
+
+    cmd = pip_ish["install", "--upgrade", "uvx"]
+    if with_uv:
+        cmd = cmd["uv"]
+
+    cmd()
+
+    new["uv"] = _get_package_version("uv", pip_ish["freeze"], default="unknown")
+
+    new["uvx"] = _get_package_version("uvx", pip_ish["freeze"], default="unknown")
+
+    return old, new
+
+
+def _self_update_via_uv(with_uv: bool):
+    return _self_update_via_cmd(_uv["pip"], with_uv=with_uv)
+
+
+def _self_update_via_pip(with_uv: bool):
+    return _self_update_via_cmd(_pip, with_uv=with_uv)
+
+
 @app.command()
 def self_update(
-    with_uv: Annotated[bool, typer.Option("--with-uv/--without-uv", '-w/-W')] = True,
+    with_uv: Annotated[bool, typer.Option("--with-uv/--without-uv", "-w/-W")] = True,
 ):
+    """Update the current installation of uvx and optionally uv."""
     # if in venv and uv available -> upgrade via uv
     # else: upgrade via pip
-    if os.getenv("VIRTUAL_ENV"):
-        print(_uv)
-    else:
-        print(_pip)
 
-    print(f'self update {with_uv = }')
+    try:
+        if os.getenv("VIRTUAL_ENV"):
+            # already activated venv
+            new, old = _self_update_via_uv(with_uv=with_uv)
+        elif sys.prefix != sys.base_prefix:
+            # venv-like environment (pipx, uvx)
+            with local.env(VIRTUAL_ENV=sys.prefix):
+                new, old = _self_update_via_uv(with_uv=with_uv)
+        else:
+            new, old = _self_update_via_pip(with_uv=with_uv)
+
+    except pb.ProcessExecutionError as e:
+        print(e.message, file=sys.stdout)
+        print(e.stdout, file=sys.stdout)
+        print(e.stderr, file=sys.stderr)
+        exit(e.retcode)
+
+    for package, old_version in old.items():
+        new_version = new.get(package)
+        if new_version == old_version:
+            rich.print(f"[bold]'{package}'[/bold] not updated (version: [green]{old_version}[/green])")
+        else:
+            rich.print(
+                f"[bold]'{package}'[/bold] updated from [red]{old_version}[/red] to [green]{new_version}[/green]"
+            )
 
 
 # list
 def _list_short(name: str, metadata: Maybe[Metadata]):
     rich.print("-", name, metadata.map_or("[red]?[/red]", lambda md: md.installed_version))
```

### Comparing `uvx-0.8.0/src/uvx/core.py` & `uvx-0.9.0/src/uvx/core.py`

 * *Files identical despite different names*

### Comparing `uvx-0.8.0/src/uvx/metadata.py` & `uvx-0.9.0/src/uvx/metadata.py`

 * *Files identical despite different names*

### Comparing `uvx-0.8.0/LICENSE.txt` & `uvx-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uvx-0.8.0/README.md` & `uvx-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `uvx-0.8.0/pyproject.toml` & `uvx-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "typer",
     "plumbum",
     "threadful>=0.3",
     "rich",
     "msgspec",
     "packaging",
     "result",
+    "configuraptor",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch",
     "python-semantic-release<8",
     "black",
```

### Comparing `uvx-0.8.0/PKG-INFO` & `uvx-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvx
-Version: 0.8.0
+Version: 0.9.0
 Summary: uvx: pipx for uv
 Project-URL: Documentation, https://github.com/robinvandernoord/uvx#readme
 Project-URL: Issues, https://github.com/robinvandernoord/uvx/issues
 Project-URL: Source, https://github.com/robinvandernoord/uvx
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: configuraptor
 Requires-Dist: msgspec
 Requires-Dist: packaging
 Requires-Dist: plumbum
 Requires-Dist: result
 Requires-Dist: rich
 Requires-Dist: threadful>=0.3
 Requires-Dist: typer
```

