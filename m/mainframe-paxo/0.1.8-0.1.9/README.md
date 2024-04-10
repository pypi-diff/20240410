# Comparing `tmp/mainframe_paxo-0.1.8.tar.gz` & `tmp/mainframe_paxo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainframe_paxo-0.1.8.tar", max compression
+gzip compressed data, was "mainframe_paxo-0.1.9.tar", max compression
```

## Comparing `mainframe_paxo-0.1.8.tar` & `mainframe_paxo-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       25 2024-01-15 14:58:59.946421 mainframe_paxo-0.1.8/doreadme.md
--rw-r--r--   0        0        0     1081 2024-01-15 14:37:46.371658 mainframe_paxo-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0      891 2024-02-20 10:54:35.799365 mainframe_paxo-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      116 2024-01-25 08:45:02.530656 mainframe_paxo-0.1.8/src/mainframe_paxo/.gitattributes
--rw-r--r--   0        0        0      289 2024-01-27 13:30:01.438094 mainframe_paxo-0.1.8/src/mainframe_paxo/__init__.py
--rw-r--r--   0        0        0       53 2024-01-23 11:40:16.473560 mainframe_paxo-0.1.8/src/mainframe_paxo/__main__.py
--rw-r--r--   0        0        0     2361 2024-02-20 10:41:46.988917 mainframe_paxo-0.1.8/src/mainframe_paxo/config.py
--rw-r--r--   0        0        0    16015 2024-02-20 10:35:31.708023 mainframe_paxo-0.1.8/src/mainframe_paxo/p4.py
--rw-r--r--   0        0        0        9 2024-01-15 14:37:46.372658 mainframe_paxo-0.1.8/src/mainframe_paxo/package_data.dat
--rw-r--r--   0        0        0   209762 2024-01-25 18:38:53.183303 mainframe_paxo-0.1.8/src/mainframe_paxo/paxo.ico
--rw-r--r--   0        0        0     3877 2024-02-20 10:52:13.287584 mainframe_paxo-0.1.8/src/mainframe_paxo/paxo.py
--rw-r--r--   0        0        0     6240 2024-01-25 08:45:02.544666 mainframe_paxo-0.1.8/src/mainframe_paxo/py.py
--rw-r--r--   0        0        0    12203 2024-02-20 10:35:31.718516 mainframe_paxo-0.1.8/src/mainframe_paxo/registry.py
--rw-r--r--   0        0        0       43 2024-01-15 14:37:46.372658 mainframe_paxo-0.1.8/src/mainframe_paxo/simple.py
--rw-r--r--   0        0        0     7405 2024-02-20 10:50:39.510920 mainframe_paxo-0.1.8/src/mainframe_paxo/tools.py
--rw-r--r--   0        0        0    27032 2024-02-20 10:35:31.729692 mainframe_paxo-0.1.8/src/mainframe_paxo/ue.py
--rw-r--r--   0        0        0        0 2024-02-20 10:35:31.733407 mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/__init__.py
--rw-r--r--   0        0        0    34016 2024-02-20 10:35:31.734046 mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/config_cache.py
--rw-r--r--   0        0        0    24056 2024-02-20 10:35:31.740315 mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/desktop.py
--rw-r--r--   0        0        0    12971 2024-02-20 10:35:31.745994 mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/desktop_win.py
--rw-r--r--   0        0        0     1211 2024-02-20 10:35:31.751974 mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/paths.py
--rw-r--r--   0        0        0     9456 2024-02-20 10:35:31.756974 mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/platform.py
--rw-r--r--   0        0        0    17884 2024-02-20 10:35:31.761974 mainframe_paxo-0.1.8/src/mainframe_paxo/uvs.py
--rw-r--r--   0        0        0     8556 2024-02-20 10:35:31.762975 mainframe_paxo-0.1.8/src/mainframe_paxo/uvs_gui.py
--rw-r--r--   0        0        0     2847 2024-02-20 10:35:31.767976 mainframe_paxo-0.1.8/src/mainframe_paxo/vstudio.py
--rw-r--r--   0        0        0      258 2024-01-25 11:51:38.034157 mainframe_paxo-0.1.8/src/mainframe_paxo/winget.py
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 mainframe_paxo-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-01-15 14:58:59.946421 mainframe_paxo-0.1.9/doreadme.md
+-rw-r--r--   0        0        0     1081 2024-01-15 14:37:46.371658 mainframe_paxo-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0      891 2024-02-20 11:30:35.464506 mainframe_paxo-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-01-25 08:45:02.530656 mainframe_paxo-0.1.9/src/mainframe_paxo/.gitattributes
+-rw-r--r--   0        0        0      289 2024-01-27 13:30:01.438094 mainframe_paxo-0.1.9/src/mainframe_paxo/__init__.py
+-rw-r--r--   0        0        0       53 2024-01-23 11:40:16.473560 mainframe_paxo-0.1.9/src/mainframe_paxo/__main__.py
+-rw-r--r--   0        0        0     2361 2024-02-20 10:41:46.988917 mainframe_paxo-0.1.9/src/mainframe_paxo/config.py
+-rw-r--r--   0        0        0    16023 2024-02-20 11:16:44.525064 mainframe_paxo-0.1.9/src/mainframe_paxo/p4.py
+-rw-r--r--   0        0        0        9 2024-01-15 14:37:46.372658 mainframe_paxo-0.1.9/src/mainframe_paxo/package_data.dat
+-rw-r--r--   0        0        0   209762 2024-01-25 18:38:53.183303 mainframe_paxo-0.1.9/src/mainframe_paxo/paxo.ico
+-rw-r--r--   0        0        0     4184 2024-02-20 11:30:03.268055 mainframe_paxo-0.1.9/src/mainframe_paxo/paxo.py
+-rw-r--r--   0        0        0     6240 2024-01-25 08:45:02.544666 mainframe_paxo-0.1.9/src/mainframe_paxo/py.py
+-rw-r--r--   0        0        0    12203 2024-02-20 10:35:31.718516 mainframe_paxo-0.1.9/src/mainframe_paxo/registry.py
+-rw-r--r--   0        0        0       43 2024-01-15 14:37:46.372658 mainframe_paxo-0.1.9/src/mainframe_paxo/simple.py
+-rw-r--r--   0        0        0     7446 2024-02-20 11:30:03.271012 mainframe_paxo-0.1.9/src/mainframe_paxo/tools.py
+-rw-r--r--   0        0        0    27718 2024-02-20 11:30:03.273974 mainframe_paxo-0.1.9/src/mainframe_paxo/ue.py
+-rw-r--r--   0        0        0        0 2024-02-20 10:35:31.733407 mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/__init__.py
+-rw-r--r--   0        0        0    34016 2024-02-20 10:35:31.734046 mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/config_cache.py
+-rw-r--r--   0        0        0    24056 2024-02-20 10:35:31.740315 mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/desktop.py
+-rw-r--r--   0        0        0    12970 2024-02-20 11:30:03.272925 mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/desktop_win.py
+-rw-r--r--   0        0        0     1211 2024-02-20 10:35:31.751974 mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/paths.py
+-rw-r--r--   0        0        0     9456 2024-02-20 10:35:31.756974 mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/platform.py
+-rw-r--r--   0        0        0    17942 2024-02-20 11:30:03.272399 mainframe_paxo-0.1.9/src/mainframe_paxo/uvs.py
+-rw-r--r--   0        0        0     8556 2024-02-20 10:35:31.762975 mainframe_paxo-0.1.9/src/mainframe_paxo/uvs_gui.py
+-rw-r--r--   0        0        0     2847 2024-02-20 10:35:31.767976 mainframe_paxo-0.1.9/src/mainframe_paxo/vstudio.py
+-rw-r--r--   0        0        0      258 2024-01-25 11:51:38.034157 mainframe_paxo-0.1.9/src/mainframe_paxo/winget.py
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 mainframe_paxo-0.1.9/PKG-INFO
```

### Comparing `mainframe_paxo-0.1.8/LICENSE.txt` & `mainframe_paxo-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/pyproject.toml` & `mainframe_paxo-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mainframe-paxo"
-version = "0.1.8"
+version = "0.1.9"
 description = "A simple CLI for paxing"
 license = "Proprietary"
 authors = ["Your Name <you@example.com>"]
 readme = "doreadme.md"
 packages = [{include = "mainframe_paxo", from = "src"}]
 include = ["*.ico"]
```

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/config.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/config.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/p4.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/p4.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 )
 @click.option(
     "--work-drive",
     type=str,
     required=True,
     prompt="Specify your work drive (e.g. D:)",
     callback=validate_work_drive,
-    default=tools.workdrive_get(empty_ok=True),
+    default=lambda: tools.workdrive_get(empty_ok=True),
 )
 @click.option(
     "--username",
     type=str,
     prompt="Perforce username",
     default=lambda: get_username(),
     help="specify the Perforce user name",
```

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/paxo.ico` & `mainframe_paxo-0.1.9/src/mainframe_paxo/paxo.ico`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/paxo.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/paxo.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,21 +17,37 @@
 def cli(ctx, verbose):
     ctx.ensure_object(dict)
     ctx.obj["verbose"] = verbose
 
 
 @cli.command()
 def initial_setup():
-    print("welcome to initial_setup_paxo")
+    click.echo("Welcome to the initial setup of paxo.")
+    click.echo(
+        """
+    Currently this is not automated.  Run the following commands:
+    - paxo p4 install
+    - paxo p4 setup
+
+    Then, run the following to sync all depots:
+    - paxo p4 sync
+
+    Then, set up various UE things:
+    - paxo ue setup
+
+    """
+    )
+
 
 @cli.group()
 def self():
     """work with paxo itself."""
     pass
 
+
 @self.command()
 def update():
     """Update paxo."""
     # rye manages our paxo installation
     # it doesn't have an "update" command, so we uninstall and install
     subprocess.run(["rye", "tools", "install", "-f", "mainframe-paxo"], check=True)
     # subprocess.run("pipx upgrade mainframe-paxo", shell=True, check=True)
```

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/py.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/py.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/registry.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/registry.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/tools.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 def env_var_get(name):
     if name in os.environ:
         return os.environ[name]
 
     # the env var may have been set in a previous session
     # and not yet updated in _out_ environment. so we look
     # in the registry.
-    with Key.current_userr("Environment") as key:
+    with Key.current_user("Environment") as key:
         value = key.get(name, None)
         if value:
             return value
     # try the system environment
     with Key.local_machine(
         "SYSTEM\\CurrentControlSet\\Control\\Session Manager\\Environment"
     ) as key:
@@ -90,15 +90,15 @@
             del os.environ[name]
         except KeyError:
             pass
     if not permanent:
         return
 
     if system:
-        key = Key.current_userr("Environment")
+        key = Key.current_user("Environment")
     else:
         key = Key.local_machine(
             "SYSTEM\\CurrentControlSet\\Control\\Session Manager\\Environment"
         )
     with key:
         try:
             del key[name]
@@ -126,19 +126,23 @@
     # W:\.paxo   # this is a marker file to identify it.
     # W:\paxdei
     # W:\UE
     # W:\otherstuff
 
     work_drive = work_drive or workdrive_get(empty_ok=False)
     drive = subst_drive_get()
-    
+
     if subst_drive == "P:":
-        raise ValueError("Drive P: is reserved for Pipeline.  Please select another drive.")
+        raise ValueError(
+            "Drive P: is reserved for Pipeline.  Please select another drive."
+        )
     if work_drive == drive:
-        raise ValueError(f"You must have a different drive letter for subst drive and work drive.  Call for help.")
+        raise ValueError(
+            "You must have a different drive letter for subst drive and work drive.  Call for help."
+        )
 
     # ensure the src folder exists
     src = os.path.join(work_drive, config.work_drive_dev_folder)
     os.makedirs(src, exist_ok=True)
 
     # ensure that it contains the .paxo file
     with open(os.path.join(src, ".paxo"), "w") as f:
```

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/ue.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/ue.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import winreg
 from contextlib import contextmanager
 
 import click
 from click import echo, secho
 
-from . import p4, tools
+from . import p4, tools, uvs
 from .registry import Key
 from .uebase import desktop
 from .uebase.desktop import is_valid_root_directory
 
 
 # helper to close winreg keys
 @contextmanager
@@ -219,16 +219,19 @@
 
     # register the engine
     if not os.path.isfile(os.path.join(engine_path, "build_info.json")):
         raise click.ClickException(
             f"Engine path {engine_path} does not contain an engine.  Have you performed a sync?"
         )
 
-    register_uproject_handler(engine_path)
-    register_engine(engine_path)
+    uvs.update_file_associations(user=True)
+    engine_id = get_engine_id_from_build_info(engine_path)
+    uvs.register_current_engine_directory(engine_root=engine_path, engine_id=engine_id)
+    # register_uproject_handler(engine_path)
+    # register_engine(engine_path)
 
     # install prerequisites
     install_prerequisites(engine_path)
 
 
 def set_location(location):
     # set the env vars related to location
@@ -505,14 +508,29 @@
     if user:
         Key(
             reg_root,
             "SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\Explorer\\FileExts\\.uproject\\UserChoice",
         ).delete(tree=True)
 
 
+def get_engine_id_from_build_info(engine_path, check=True):
+    # read the engine registry name from the build_info.json file
+    check = True
+
+    if check and not is_valid_root_directory(engine_path):
+        raise click.ClickException(f"Engine path {engine_path} is not valid")
+
+    try:
+        with open(os.path.join(engine_path, "build_info.json")) as f:
+            info = json.load(f)
+        return info["engine_id"]
+    except OSError:
+        return None
+
+
 def register_engine(engine_path, engine_id=None, check=True):
     # read the engine registry name from the build_info.json file
 
     if check and not is_valid_root_directory(engine_path):
         raise click.ClickException(f"Engine path {engine_path} is not valid")
 
     if not engine_id:
```

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/config_cache.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/config_cache.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/desktop.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/desktop.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/desktop_win.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/desktop_win.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     with root.create(".uproject") as key:
         key[""] = "Unreal.ProjectFile"
         print(key[""])
 
     with root.create("Unreal.ProjectFile") as key:
         # we could well clear this subtree first and write it all fresh
         key[""] = "Unreal Engine Project File"
-        print (key[""])
+        print(key[""])
         key["VersionSelectorExecutable"] = handler
 
         # the DefaultIcon subkey, used for the shell in the file
         with key.create("DefaultIcon") as subkey:
             subkey[""] = fileicon
 
         with key.create("shell") as subkey:
```

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/paths.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/paths.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/uebase/platform.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/uebase/platform.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/uvs.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/uvs.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     help="The engine root to register",
 )
 def register(engine_id, unattended, engine_root):
     """Register a _this_ engine.  Not supported."""
     register_current_engine_directory(engine_id, unattended, engine_root)
 
 
-def register_current_engine_directory(engine_id, unattended, engine_root):
+def register_current_engine_directory(
+    engine_id=None, unattended=False, engine_root=None
+):
     if not engine_root:
         abort("can't register _this_engine, because this is a standalone tool")
     engine_root = os.path.abspath(engine_root)
     if not desktop.is_valid_root_directory(engine_root):
         abort(f"Invalid engine root {engine_root}")
 
     if not engine_id:
@@ -122,15 +124,17 @@
     elif clear:
         desktop.platform.clear_file_associations(user=user)
         click.echo(
             f"File associations cleared for scope {'user' if user else 'machine'}"
         )
     else:
         if engine_root:
-            desktop.platform.update_file_associations(engine_root=engine_root, verify=True)
+            desktop.platform.update_file_associations(
+                engine_root=engine_root, verify=True
+            )
         else:
             handler = find_run_args(gui=True)
             desktop.platform.update_file_associations(handler=handler, verify=True)
         click.echo(
             f"File associations updated for scope {'user' if user else 'machine'}"
         )
 
@@ -366,15 +370,15 @@
             return False
         return True
     finally:
         if window:
             window.close()
 
 
-@cli.command()
+# @cli.command()
 def register_test():
     """Register uvs as the default UnrealVersionSelector"""
     print(sys.argv)
     print(__spec__)
     print(sys.executable)
     return
     # find the command used to run us
```

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/uvs_gui.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/uvs_gui.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/src/mainframe_paxo/vstudio.py` & `mainframe_paxo-0.1.9/src/mainframe_paxo/vstudio.py`

 * *Files identical despite different names*

### Comparing `mainframe_paxo-0.1.8/PKG-INFO` & `mainframe_paxo-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mainframe-paxo
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple CLI for paxing
 License: Proprietary
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

