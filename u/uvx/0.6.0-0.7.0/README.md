# Comparing `tmp/uvx-0.6.0.tar.gz` & `tmp/uvx-0.7.0.tar.gz`

## Comparing `uvx-0.6.0.tar` & `uvx-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 uvx-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_constants.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_maybe.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_python.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_symlinks.py
--rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/cli.py
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/core.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.6.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.6.0/README.md
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 uvx-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 uvx-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 uvx-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_constants.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_maybe.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_python.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/_symlinks.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/cli.py
+-rw-r--r--   0        0        0    15071 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/core.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.7.0/src/uvx/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.7.0/README.md
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 uvx-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 uvx-0.7.0/PKG-INFO
```

### Comparing `uvx-0.6.0/CHANGELOG.md` & `uvx-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.7.0 (2024-04-10)
+
+### Feature
+
+* `uvx upgrade-all` ([`5edc7af`](https://github.com/robinvandernoord/uvx/commit/5edc7afeda4bb544b346f962a730f66c6b92dbf8))
+
+### Fix
+
+* Make linters etc happy ([`bc16251`](https://github.com/robinvandernoord/uvx/commit/bc16251ac58221131f1192ea78fc95f80650421f))
+
 ## v0.6.0 (2024-04-05)
 
 ### Feature
 
 * Implemented  first version of `uvx upgrade` ([`ffcb73a`](https://github.com/robinvandernoord/uvx/commit/ffcb73ad928f089ef3c0c3705b00fc04c840c9ff))
 * Work in progress on uvx upgrade ([`d48524a`](https://github.com/robinvandernoord/uvx/commit/d48524adf5a9a08ae4d4b8485789ff33e937f278))
```

### Comparing `uvx-0.6.0/src/uvx/_python.py` & `uvx-0.7.0/src/uvx/_python.py`

 * *Files identical despite different names*

### Comparing `uvx-0.6.0/src/uvx/_symlinks.py` & `uvx-0.7.0/src/uvx/_symlinks.py`

 * *Files identical despite different names*

### Comparing `uvx-0.6.0/src/uvx/cli.py` & `uvx-0.7.0/src/uvx/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This file builds the Typer cli."""
 
 import os
 import subprocess  # nosec
 import sys
 from datetime import datetime
 from pathlib import Path
-from typing import Optional
+from typing import Annotated
 
 import rich
 import typer
 from result import Err, Ok, Result
 from typer import Context
 
 from uvx._constants import BIN_DIR
@@ -30,48 +30,81 @@
 )
 from .metadata import Metadata
 
 app = typer.Typer()
 
 
 def output(result: Result[str, Exception]) -> None:
+    """Output positive (ok) result to stdout and error result to stderr."""
     match result:
         case Ok(msg):
-            rich.print(msg)  # :trash:
+            rich.print(msg)
         case Err(err):
             rich.print(err, file=sys.stderr)
 
 
+OPTION_PYTHON_HELP_TEXT = "Python version or executable to use, e.g. `3.12`, `python3.12`, `/usr/bin/python3.12`"
+
+
 @app.command()
-def install(package_name: str, force: bool = False, python: str = "", no_cache: bool = False):
+def install(
+    package_name: str,
+    force: Annotated[
+        bool,
+        typer.Option(
+            "-f", "--force", help="Overwrite currently installed executables with the same name (in ~/.local/bin)"
+        ),
+    ] = False,
+    python: Annotated[str, typer.Option(help=OPTION_PYTHON_HELP_TEXT)] = "",
+    no_cache: Annotated[bool, typer.Option("--no-cache", help="Run without `uv` cache")] = False,
+):
     """Install a package (by pip name)."""
-    # todo: support 'install .'
     output(install_package(package_name, python=python, force=force, no_cache=no_cache))
 
 
 @app.command(name="upgrade")
 @app.command(name="update")
-def upgrade(package_name: str, force: bool = False, skip_injected: bool = False, no_cache: bool = False):
+def upgrade(
+    package_name: str,
+    force: Annotated[bool, typer.Option("-f", "--force", help="Ignore previous version constraint")] = False,
+    skip_injected: Annotated[
+        bool, typer.Option("--skip-injected", help="Don't also upgrade injected packages")
+    ] = False,
+    no_cache: Annotated[bool, typer.Option("--no-cache", help="Run without `uv` cache")] = False,
+):
+    """Upgrade a package."""
     output(upgrade_package(package_name, force=force, skip_injected=skip_injected, no_cache=no_cache))
 
 
 @app.command(name="remove")
 @app.command(name="uninstall")
-def uninstall(package_name: str, force: bool = False):
+def uninstall(
+    package_name: str,
+    force: Annotated[
+        bool,
+        typer.Option(
+            "-f",
+            "--force",
+            help="Remove executable with the same name (in ~/.local/bin) even if related venv was not found",
+        ),
+    ] = False,
+):
     """Uninstall a package (by pip name)."""
     output(uninstall_package(package_name, force=force).map(lambda version: f"🗑️ {package_name}{version} removed!"))
 
 
 @app.command()
 def reinstall(
     package: str,
-    python: Optional[str] = None,
-    force: bool = False,
-    without_injected: bool = False,
-    no_cache: bool = False,
+    python: Annotated[str, typer.Option(help=OPTION_PYTHON_HELP_TEXT)] = "",
+    force: Annotated[bool, typer.Option("-f", "--force", help="See `install --force`")] = False,
+    without_injected: Annotated[
+        bool, typer.Option("--without-injected", help="Don't include previously injected libraries in reinstall")
+    ] = False,
+    no_cache: Annotated[bool, typer.Option("--no-cache", help="Run without `uv` cache")] = False,
 ):
     """Uninstall a package (by pip name) and re-install from the original spec (unless a new spec is supplied)."""
     output(
         reinstall_package(
             package,
             python=python,
             force=force,
@@ -79,22 +112,46 @@
             no_cache=no_cache,
         ).map(lambda _: _.replace(" installed", " reinstalled"))
     )
 
 
 @app.command()
 def inject(into: str, package_specs: list[str]):
+    """Install additional packages to a virtual environment managed by uvx."""
     output(
         inject_packages(
             into,
             set(package_specs),
         )
     )
 
 
+# todo:
+# self-upgrade (uv and uvx)
+# upgrade-all
+
+@app.command()
+def upgrade_all(
+    force: Annotated[bool, typer.Option("-f", "--force", help="Ignore previous version constraint")] = False,
+    skip_injected: Annotated[
+        bool, typer.Option("--skip-injected", help="Don't also upgrade injected packages")
+    ] = False,
+    no_cache: Annotated[bool, typer.Option("--no-cache", help="Run without `uv` cache")] = False,
+):
+    """Upgrade all uvx-installed packages."""
+
+    for (venv_name, _) in list_packages():
+        upgrade(
+            venv_name,
+            force=force,
+            skip_injected=skip_injected,
+            no_cache=no_cache
+        )
+
+
 # list
 def _list_short(name: str, metadata: Maybe[Metadata]):
     rich.print("-", name, metadata.map_or("[red]?[/red]", lambda md: md.installed_version))
 
 
 TAB = " " * 3
 
@@ -174,19 +231,14 @@
 def runpython(venv: str, ctx: Context):
     """Run 'python' in the right venv."""
     with as_virtualenv(venv) as venv_path:
         python = venv_path / "bin" / "python"
         subprocess.run([python, *ctx.args])  # nosec
 
 
-# todo:
-# self-upgrade (uv and uvx)
-# upgrade-all
-
-
 def add_to_bashrc(text: str, with_comment: bool = True):
     """Add text to ~/.bashrc, usually with a comment (uvx + timestamp)."""
     with (Path.home() / ".bashrc").resolve().open("a") as f:
         now = str(datetime.now()).split(".")[0]
         final_text = "\n"
         final_text += f"# Added by `uvx` at {now}\n" if with_comment else ""
         final_text += text + "\n"
```

### Comparing `uvx-0.6.0/src/uvx/core.py` & `uvx-0.7.0/src/uvx/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,58 +107,59 @@
 
 
 def install_package(
     package_name: str,
     venv: Optional[Path] = None,
     python: Optional[str] = None,
     force: bool = False,
-    extras: Optional[list[str]] = None,
+    extras: Optional[typing.Iterable[str]] = None,
     no_cache: bool = False,
 ) -> Result[str, Exception]:
     """
     Install a package in a virtual environment.
 
     Args:
         package_name (str): The name of the package.
         venv (Optional[Path], optional): The path of the virtual environment. Defaults to None.
+        python (str): version or executable to use.
         force (bool, optional): If True, overwrites existing package. Defaults to False.
+        extras: which optional features ('extras') to install for this package.
+        no_cache: don't use `uv` cache.
     """
     if extras is None:
         extras = []
 
     match collect_metadata(package_name):
         case Err(e):
             return Err(e)
         case Ok(meta):
             # just bind meta
             ...
 
     if venv is None:
         venv = create_venv(meta.name, python=python, force=force)
 
-    # todo: make --force use --no-cache
-
     with virtualenv(venv), exit_on_pb_error():
-        try:
-            args = []
-            text = f"installing {meta.name}"
-            if extras:
-                args.extend(extras)
-                text += f" with {extras}"
+        args: list[str] = []
+        text = f"installing {meta.name}"
+        if extras:
+            args.extend(extras)
+            text += f" with {extras}"
 
-            if no_cache:
-                args += ["--no-cache"]
+        if no_cache or force:
+            args += ["--no-cache"]
 
+        try:
             animate(uv("pip", "install", meta.install_spec, *args), text=text)
 
-            # must still be in the venv for these:
+            # must still be in the venv and try for these:
             meta.installed_version = get_package_version(meta.name, venv)
             meta.python = get_python_version(venv)
             meta.python_raw = get_python_executable(venv)
-            meta.injected = extras
+            meta.injected = set(extras)
 
         except plumbum.ProcessExecutionError as e:
             remove_dir(venv)
             return Err(e)
 
     msg = ""
     if install_symlinks(meta.name, venv, force=force, meta=meta):
@@ -185,14 +186,16 @@
     spec. The Python version used for the virtual environment can be specified. If not specified, it uses the Python
     version from the existing metadata if available.
 
     Args:
         package_name (str): The name of the package to reinstall.
         python (Optional[str], optional): The Python version to use for the virtual environment. Defaults to None.
         force (bool, optional): If True, ignores if the virtual environment does not exist. Defaults to False.
+        with_injected (bool): also re-include injected packages?
+        no_cache: don't use `uv` cache.
 
     Raises:
         SystemExit: If the package is not installed in the virtual environment and force is False.
     """
     match collect_metadata(package_name):
         case Err(e):
             # can't work without metadata, just stop
@@ -223,22 +226,23 @@
         case (False, Ok(metadata)):
             install_spec = metadata.install_spec
         case _:
             # if new install spec is True or there is no old metadata:
             install_spec = package_name
 
     # python = python or (existing_metadata.python_raw if existing_metadata else None)
-    python = python or existing_metadata.map_or(None, lambda metadata: metadata.python_raw)
+    python = python or existing_metadata.map_or(None, lambda m: m.python_raw)
 
     uninstall_package(new_metadata.name, force=force)
     extras = metadata.injected if (with_injected and metadata and metadata.injected) else []
     return install_package(install_spec, python=python, force=force, extras=extras, no_cache=no_cache)
 
 
 def inject_packages(into: str, package_specs: set[str]) -> Result[str, Exception]:
+    """Install extra libraries into a package-specific venv."""
     match collect_metadata(into):
         case Err(e):
             return Err(e)
         case Ok(meta):
             # just bind meta
             ...
 
@@ -273,14 +277,15 @@
     if path.exists():
         shutil.rmtree(path)
 
 
 def upgrade_package(
     package_name: str, force: bool = False, skip_injected: bool = False, no_cache: bool = False
 ) -> Result[str, Exception]:
+    """Upgrade a package in its venv."""
     # run `uv pip install --upgrade package` with requested install spec (version, extras, injected)
     # if --force is used, the previous version is ignored.
     match collect_metadata(package_name):
         case Err(e):
             return Err(e)
         case Ok(spec_metadata):
             # bind spec_metadata
@@ -298,16 +303,21 @@
 
     with virtualenv(venv), exit_on_pb_error():
         # pip upgrade package[extras]==version *injected
         # if version spec in spec_metadata use that instead
         # if --force, drop version spec
         base_pkg = meta.name
         extras = meta.extras
-        injected = [] if skip_injected else (meta.injected or [])
-        version = spec_metadata.requested_version or ("" if force else meta.requested_version)
+
+        injected: set[str] = (not skip_injected and meta.injected) or set()
+        # injected = set() if skip_injected else (meta.injected or set())
+
+        version: str = spec_metadata.requested_version or (not force and meta.requested_version) or ""
+        # version = spec_metadata.requested_version or ("" if force else meta.requested_version)
+
         options = []
         if force:
             options.append("--no-cache")
 
         upgrade_spec = base_pkg + version
         if extras:
             upgrade_spec += "[" + ",".join(extras) + "]"
@@ -318,18 +328,18 @@
             return Err(e)
 
         meta.requested_version = version
         new_version = meta.installed_version = get_package_version(meta.name, venv)
         store_metadata(meta, venv)
 
     if old_version == new_version:
-        # todo: if meta.requested_version - warn
         msg = f"🌟 '{package_name}' is already up to date at version {new_version}!"
         if meta.requested_version:
-            msg += f"\n💡 This package was installed with a version constraint ({meta.requested_version}). If you want to ignore this constraint, use `uvx upgrade --force {package_name}`."
+            msg += (f"\n💡 This package was installed with a version constraint ({meta.requested_version}). "
+                    f"If you want to ignore this constraint, use `uvx upgrade --force {package_name}`.")
 
     else:
         msg = f"🚀 Successfully updated '{package_name}' from version {old_version} to version {new_version}!"
 
     return Ok(msg)
 
 
@@ -344,28 +354,29 @@
     workdir = ensure_local_folder()
     venv_path = workdir / "venvs" / package_name
 
     if not venv_path.exists() and not force:
         escaped = package_name.replace("[", "\\[")
         return Err(
             NotADirectoryError(
-                f"No virtualenv for '{escaped}', stopping. Use '--force' to remove an executable with that name anyway.",
+                f"No virtualenv for '{escaped}', stopping. "
+                f"Use '--force' to remove an executable with that name anyway.",
             )
         )
 
     meta = read_metadata(venv_path)
 
     symlinks = find_symlinks(package_name, venv_path) or [package_name]
 
     for symlink in symlinks:
         remove_symlink(symlink)
 
     remove_dir(venv_path)
 
-    _version = meta.map_or("", lambda meta: f" ({meta.installed_version})")
+    _version = meta.map_or("", lambda m: f" ({m.installed_version})")
     return Ok(_version)
 
 
 def ensure_local_folder() -> Path:
     """
     Ensure the local folder exists.
 
@@ -380,14 +391,15 @@
     """
     Create a virtual environment.
 
     Args:
         name (str): The name of the virtual environment.
         python (str): which version of Python to use (e.g. 3.11, python3.11)
         force (bool): ignore existing venv
+        with_pip (bool): also install (regular) pip into the venv? (required for `uvx runpip`)
 
     Returns:
         Path: The path of the virtual environment.
     """
     workdir = ensure_local_folder()
 
     venv_path = workdir / "venvs" / name
```

### Comparing `uvx-0.6.0/src/uvx/metadata.py` & `uvx-0.7.0/src/uvx/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,24 +60,26 @@
 
 
 encoder = msgspec.msgpack.Encoder()
 decoder = msgspec.msgpack.Decoder(type=Metadata)
 
 
 def fake_install(spec: str) -> dict:
+    """Dry run pip to extract metadata of a local package."""
     _uv("pip", "install", "pip")  # ensure we have pip
 
     with tempfile.NamedTemporaryFile() as f:
         _pip("install", "--no-deps", "--dry-run", "--ignore-installed", "--report", f.name, spec)
 
         return json.load(f)
 
 
 @threadful.thread
 def resolve_local(spec: str) -> tuple[Maybe[str], Maybe[str]]:
+    """Resolve the package name of a local package by dry run installing it."""
     try:
         full_data = fake_install(spec)
         install_data = full_data["install"][0]
 
         name = install_data["metadata"]["name"]
         extras = install_data.get("requested_extras")
         file_url = install_data["download_info"]["url"]
```

### Comparing `uvx-0.6.0/LICENSE.txt` & `uvx-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uvx-0.6.0/README.md` & `uvx-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `uvx-0.6.0/pyproject.toml` & `uvx-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-0.6.0/PKG-INFO` & `uvx-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: uvx
-Version: 0.6.0
+Version: 0.7.0
 Summary: uvx: pipx for uv
 Project-URL: Documentation, https://github.com/robinvandernoord/uvx#readme
 Project-URL: Issues, https://github.com/robinvandernoord/uvx/issues
 Project-URL: Source, https://github.com/robinvandernoord/uvx
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

