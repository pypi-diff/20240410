# Comparing `tmp/unknown-cli-0.9.3.tar.gz` & `tmp/unknown-cli-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unknown-cli-0.9.3.tar", last modified: Fri Apr  5 17:28:53 2024, max compression
+gzip compressed data, was "unknown-cli-0.9.4.tar", last modified: Tue Apr  9 18:01:03 2024, max compression
```

## Comparing `unknown-cli-0.9.3.tar` & `unknown-cli-0.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.491376 unknown-cli-0.9.3/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-05 17:28:53.489375 unknown-cli-0.9.3/PKG-INFO
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       30 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/README.md
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       38 2024-04-05 17:28:53.491376 unknown-cli-0.9.3/setup.cfg
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2695 2024-03-13 22:40:13.000000 unknown-cli-0.9.3/setup.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.353945 unknown-cli-0.9.3/unknown_cli.egg-info/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      561 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        1 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       83 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      130 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/requires.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       11 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/top_level.txt
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.408944 unknown-cli-0.9.3/unknowncli/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        5 2024-04-04 23:22:42.000000 unknown-cli-0.9.3/unknowncli/VERSION
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      407 2024-03-11 22:54:16.000000 unknown-cli-0.9.3/unknowncli/__init__.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1815 2024-04-04 23:21:31.000000 unknown-cli-0.9.3/unknowncli/__main__.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.466654 unknown-cli-0.9.3/unknowncli/commands/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/unknowncli/commands/__init__.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    34140 2024-03-22 11:18:20.000000 unknown-cli-0.9.3/unknowncli/commands/preflight.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    19657 2024-04-04 23:22:04.000000 unknown-cli-0.9.3/unknowncli/commands/project.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    18247 2024-04-04 23:22:04.000000 unknown-cli-0.9.3/unknowncli/commands/task.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2436 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/unknowncli/commands/unreal.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.478611 unknown-cli-0.9.3/unknowncli/data/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     3560 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/unknowncli/data/.p4ignore.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      840 2023-12-07 23:07:53.000000 unknown-cli-0.9.3/unknowncli/set_registry_keys.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1005 2023-12-07 23:07:53.000000 unknown-cli-0.9.3/unknowncli/set_url_handler.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    11456 2024-04-04 23:21:31.000000 unknown-cli-0.9.3/unknowncli/utils.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2024-04-09 18:01:03.406341 unknown-cli-0.9.4/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2024-04-09 18:01:03.404769 unknown-cli-0.9.4/PKG-INFO
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       28 2023-07-05 17:33:30.000000 unknown-cli-0.9.4/README.md
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       38 2024-04-09 18:01:03.406865 unknown-cli-0.9.4/setup.cfg
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     2594 2023-08-31 11:44:27.000000 unknown-cli-0.9.4/setup.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2024-04-09 18:01:03.219271 unknown-cli-0.9.4/unknown_cli.egg-info/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2024-04-09 18:01:02.000000 unknown-cli-0.9.4/unknown_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      561 2024-04-09 18:01:03.000000 unknown-cli-0.9.4/unknown_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        1 2024-04-09 18:01:02.000000 unknown-cli-0.9.4/unknown_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       83 2024-04-09 18:01:02.000000 unknown-cli-0.9.4/unknown_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      130 2024-04-09 18:01:02.000000 unknown-cli-0.9.4/unknown_cli.egg-info/requires.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       11 2024-04-09 18:01:02.000000 unknown-cli-0.9.4/unknown_cli.egg-info/top_level.txt
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2024-04-09 18:01:03.291450 unknown-cli-0.9.4/unknowncli/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        5 2024-04-09 18:01:02.000000 unknown-cli-0.9.4/unknowncli/VERSION
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      391 2023-10-03 08:47:00.000000 unknown-cli-0.9.4/unknowncli/__init__.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     1815 2024-04-09 17:39:46.000000 unknown-cli-0.9.4/unknowncli/__main__.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2024-04-09 18:01:03.372005 unknown-cli-0.9.4/unknowncli/commands/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2022-10-25 14:43:45.000000 unknown-cli-0.9.4/unknowncli/commands/__init__.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    34140 2024-04-09 17:39:46.000000 unknown-cli-0.9.4/unknowncli/commands/preflight.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    19661 2024-04-09 18:00:18.000000 unknown-cli-0.9.4/unknowncli/commands/project.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    18247 2024-04-09 17:39:46.000000 unknown-cli-0.9.4/unknowncli/commands/task.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     2349 2023-10-03 08:47:01.000000 unknown-cli-0.9.4/unknowncli/commands/unreal.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2024-04-09 18:01:03.387746 unknown-cli-0.9.4/unknowncli/data/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     3408 2023-10-03 08:47:01.000000 unknown-cli-0.9.4/unknowncli/data/.p4ignore.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      840 2024-01-23 13:34:58.000000 unknown-cli-0.9.4/unknowncli/set_registry_keys.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     1005 2024-01-23 13:34:58.000000 unknown-cli-0.9.4/unknowncli/set_url_handler.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    11460 2024-04-09 18:00:39.000000 unknown-cli-0.9.4/unknowncli/utils.py
```

### Comparing `unknown-cli-0.9.3/unknown_cli.egg-info/SOURCES.txt` & `unknown-cli-0.9.4/unknown_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.3/unknowncli/__main__.py` & `unknown-cli-0.9.4/unknowncli/__main__.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.3/unknowncli/commands/preflight.py` & `unknown-cli-0.9.4/unknowncli/commands/preflight.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.3/unknowncli/commands/project.py` & `unknown-cli-0.9.4/unknowncli/commands/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             import winreg
             echo(f"Adding Virtual Drive {SUBST_DRIVE} -> {perforce_path} to startup")
             h = winreg.CreateKey(winreg.HKEY_LOCAL_MACHINE, "Software\\Microsoft\\Windows\\CurrentVersion\\Run")
             winreg.SetValueEx(h, "Perforce Work Drive", 0, winreg.REG_SZ, subst_cmd)
         except:
             secho("Access denied setting subst registry key. Running elevated process...")
             path = Path(__file__).parent.parent / "set_registry_keys.py"
-            cmd = f"{sys.executable} {path.resolve()} \"{subst_cmd}\""
+            cmd = f"{sys.executable} \"{path.resolve()}\" \"{subst_cmd}\""
             check_call(cmd)
 
         h = winreg.CreateKey(winreg.HKEY_CURRENT_USER, "SOFTWARE\\perforce\\environment")
         winreg.SetValueEx(h, "P4CONFIG", 0, winreg.REG_SZ, str(config_file))
 
         if not perforce_path.exists():
             abort(f"Failed to add subst for {SUBST_DRIVE}")
```

### Comparing `unknown-cli-0.9.3/unknowncli/commands/task.py` & `unknown-cli-0.9.4/unknowncli/commands/task.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.3/unknowncli/commands/unreal.py` & `unknown-cli-0.9.4/unknowncli/commands/unreal.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import time 
-import requests
-import logging
-from pathlib import Path
-from ..utils import abort
-from subprocess import Popen
-import psutil
-from  urllib.parse import quote_plus
-from typer import echo, secho, Typer
-from ..utils import set_url_handler
-
-log = logging.getLogger(__name__)
-
-UNREAL_EDITOR = r"s:\sn2-main\UE\Engine\Binaries\Win64\UnrealEditor.exe s:\sn2-main\UE\Subnautica2\Subnautica2.uproject"
-EDITOR_URL = "http://127.0.0.1:8082"
-
-app = Typer()
-
-def ensure_editor_running():
-    for proc in psutil.process_iter():
-        if "UnrealEditor" in proc.name():
-            return
-    echo(f"Running editor: {UNREAL_EDITOR}")
-    Popen(UNREAL_EDITOR, shell=True)
-    time.sleep(3.0)
-    echo("Checking for response...")
-    n = 0
-    num_tries = 10
-    while n < num_tries:
-        try:
-            url = f"http://127.0.0.1:8082/"
-            resp = requests.get(url)
-            return
-        except:
-            time.sleep(1.0)
-    abort("Could not start editor.")
-
-
-@app.command()
-def diff(first, second):
-    """
-    Diff two .uasset files in the editor.
-    """
-    ensure_editor_running()
-    try:
-        first_file = Path(first)
-        second_file = Path(second)
-        if not first_file.is_file() or not second_file.is_file():
-            abort(f"{first} or {second} not found")
-        secho(f"Diffing the following files:\n  {first}\n  {second}", bold=True)
-
-        # with open("c:/temp/out.log", "w") as f:
-        #     f.write(f"Diffing the following files:\n  {first}\n  {second}")
-        left = quote_plus(first)
-        right = quote_plus(second)
-        left = first.replace("#", "%23")
-        url = f"{EDITOR_URL}/diff?left={left}&right={right}"
-        echo(url)
-        resp = requests.get(url)
-        print(resp.text)
-    except Exception as e:
-        raise
-        # with open("c:/temp/out.log", "w") as f:
-        #     f.write(str(e))
-
-@app.command()
-def asset(name):
-    """
-    Open an asset in a running editor or spawn an editor
-    """
-    ensure_editor_running()
-    p = Path(name)
-    if p.is_file():
-        asset_name = p.stem
-    else:
-        asset_name = p.name
-    print(f"Getting {asset_name}...")
-    resp = requests.get(f"{EDITOR_URL}/asset/{asset_name}")
-    print(resp.text)
-    time.sleep(5.0)
-
-@app.command()
-def handler():
-    """
-    Set the URL handler
-    """
-    set_url_handler(True)
+import time 
+import requests
+import logging
+from pathlib import Path
+from ..utils import abort
+from subprocess import Popen
+import psutil
+from  urllib.parse import quote_plus
+from typer import echo, secho, Typer
+from ..utils import set_url_handler
+
+log = logging.getLogger(__name__)
+
+UNREAL_EDITOR = r"s:\sn2-main\UE\Engine\Binaries\Win64\UnrealEditor.exe s:\sn2-main\UE\Subnautica2\Subnautica2.uproject"
+EDITOR_URL = "http://127.0.0.1:8082"
+
+app = Typer()
+
+def ensure_editor_running():
+    for proc in psutil.process_iter():
+        if "UnrealEditor" in proc.name():
+            return
+    echo(f"Running editor: {UNREAL_EDITOR}")
+    Popen(UNREAL_EDITOR, shell=True)
+    time.sleep(3.0)
+    echo("Checking for response...")
+    n = 0
+    num_tries = 10
+    while n < num_tries:
+        try:
+            url = f"http://127.0.0.1:8082/"
+            resp = requests.get(url)
+            return
+        except:
+            time.sleep(1.0)
+    abort("Could not start editor.")
+
+
+@app.command()
+def diff(first, second):
+    """
+    Diff two .uasset files in the editor.
+    """
+    ensure_editor_running()
+    try:
+        first_file = Path(first)
+        second_file = Path(second)
+        if not first_file.is_file() or not second_file.is_file():
+            abort(f"{first} or {second} not found")
+        secho(f"Diffing the following files:\n  {first}\n  {second}", bold=True)
+
+        # with open("c:/temp/out.log", "w") as f:
+        #     f.write(f"Diffing the following files:\n  {first}\n  {second}")
+        left = quote_plus(first)
+        right = quote_plus(second)
+        left = first.replace("#", "%23")
+        url = f"{EDITOR_URL}/diff?left={left}&right={right}"
+        echo(url)
+        resp = requests.get(url)
+        print(resp.text)
+    except Exception as e:
+        raise
+        # with open("c:/temp/out.log", "w") as f:
+        #     f.write(str(e))
+
+@app.command()
+def asset(name):
+    """
+    Open an asset in a running editor or spawn an editor
+    """
+    ensure_editor_running()
+    p = Path(name)
+    if p.is_file():
+        asset_name = p.stem
+    else:
+        asset_name = p.name
+    print(f"Getting {asset_name}...")
+    resp = requests.get(f"{EDITOR_URL}/asset/{asset_name}")
+    print(resp.text)
+    time.sleep(5.0)
+
+@app.command()
+def handler():
+    """
+    Set the URL handler
+    """
+    set_url_handler(True)
```

### Comparing `unknown-cli-0.9.3/unknowncli/data/.p4ignore.txt` & `unknown-cli-0.9.4/unknowncli/data/.p4ignore.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-# Here you can specify files to ignore when adding files to the depot.
-#
-# The syntax for P4IGNORE files is not the same as Perforce syntax.
-# Instead, it is similar to that used by other versioning systems:
-#
-# - Files are specified in local syntax
-# - a # character at the beginning of a line denotes a comment
-# - a ! character at the beginning of a line excludes the file specification
-# - a * wildcard matches substrings.
-#
-# http://stackoverflow.com/questions/18240084/how-does-perforce-ignore-file-syntax-differ-from-gitignore-syntax
-
-/*.sln
-/.p4sync.txt
-
-# Ignore all Visual Studio temp files.
-*.suo
-*.opensdf
-*.sdf
-.patch_*
-
-*/DerivedDataCache/
-**/DerivedDataCache/Boot.ddc
-**/DerivedDataCache/**/*.udd
-
-# Ignore all Intermediate and Saved directories
-*/Intermediate/*
-*/Saved/*
-
-# Ignore UBT's configuration.xml
-Engine/Programs/UnrealBuildTool/*
-*.uatbuildrecord
-*.tmp
-
-# Ignore built binaries and temporary build files
-*/obj/*
-*.csprojAssemblyReference.cache
-
-# Ignore UBT's log output files
-/Engine/Programs/UnrealBuildTool/*.txt
-
-# Ignore Python cached files
-*.pyc
-
-# Ignore JetBrain's IDE folders
-.idea/
-.gradle/
-
-# Ignore autogenerated files from HoloLens WMRInterop
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/packages/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/Generated Files/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/x64/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/ARM64/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/x64/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/ARM64/*
-
-Saved/
-LocalBuilds/
-*.csproj.*
-.vs/*
-.vsconfig
-*.pdb
-*.suo
-*.opensdf
-*.sdf
-*.tmp
-*.mdb
-obj/
-*.vcxproj
-*.sln
-*-Debug.*
-FileOpenOrder/
-*.xcworkspace
-*.xcodeproj
-./Makefile
-./CMakeLists.txt
-.ue4dependencies
-Samples/*
-FeaturePacks/*
-Templates/*
-Engine/Documentation/*
-
-# Engine intermediates
-Engine/Intermediate/*
-Intermediate/
-
-# Intermediate folders for programs should not be checked in
-Engine\Programs\*\Intermediate\*
-
-# Intermediate folders created for various C# programs
-Engine\Source\Programs\*\obj\*
-
-# Saved folders for programs should not be checked in
-Engine\Programs\*\Saved\*
-Engine\Programs\UnrealBuildTool\*
-
-# Derived data cache should never be checked in
-Engine/DerivedDataCache/*
-
-# Ignore any build receipts
-Engine/Build/Receipts/*
-
-# Ignore personal workspace vars
-p4config.txt
-
-# Ignore Unix backup files
-*~
-
-# Ignore Mac desktop services store files
-.DS_Store
-
-# Ignore crash reports
-crashinfo--*
-
-# Ignore linux project files
-*.user
-*.pro
-*.pri
-*.kdev4
-
-# Obj-C/Swift specific
-*.hmap
-*.ipa
-*.dSYM.zip
-*.dSYM
-
-# Ignore documentation generated for C# tools
-Engine/Binaries/DotNET/UnrealBuildTool.xml
-Engine/Binaries/DotNET/AutomationScripts/BuildGraph.Automation.xml
-
-# Ignore version files in the Engine/Binaries directory created by UBT
-/Engine/Binaries/**/*.version
-
-# Ignore exp files in the the Engine/Binaries directory as they aren't C/C++ source files
-/Engine/Binaries/**/*.exp
-
-# Ignore Swarm local save files
-Engine/Binaries/DotNET/SwarmAgent.DeveloperOptions.xml
-Engine/Binaries/DotNET/SwarmAgent.Options.xml
-
-# Intermediary Files
-*.target.xml
-*.exe.config
-*.exe.manifest
-
-# Ignore project-specific files
-*/Build/Receipts/*
-*/DerivedDataCache/*
-*/Binaries/*-Shipping.*
-*/Intermediate/*
-
-*/Logs/*
+# Here you can specify files to ignore when adding files to the depot.
+#
+# The syntax for P4IGNORE files is not the same as Perforce syntax.
+# Instead, it is similar to that used by other versioning systems:
+#
+# - Files are specified in local syntax
+# - a # character at the beginning of a line denotes a comment
+# - a ! character at the beginning of a line excludes the file specification
+# - a * wildcard matches substrings.
+#
+# http://stackoverflow.com/questions/18240084/how-does-perforce-ignore-file-syntax-differ-from-gitignore-syntax
+
+/*.sln
+/.p4sync.txt
+
+# Ignore all Visual Studio temp files.
+*.suo
+*.opensdf
+*.sdf
+.patch_*
+
+*/DerivedDataCache/
+**/DerivedDataCache/Boot.ddc
+**/DerivedDataCache/**/*.udd
+
+# Ignore all Intermediate and Saved directories
+*/Intermediate/*
+*/Saved/*
+
+# Ignore UBT's configuration.xml
+Engine/Programs/UnrealBuildTool/*
+*.uatbuildrecord
+*.tmp
+
+# Ignore built binaries and temporary build files
+*/obj/*
+*.csprojAssemblyReference.cache
+
+# Ignore UBT's log output files
+/Engine/Programs/UnrealBuildTool/*.txt
+
+# Ignore Python cached files
+*.pyc
+
+# Ignore JetBrain's IDE folders
+.idea/
+.gradle/
+
+# Ignore autogenerated files from HoloLens WMRInterop
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/packages/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/Generated Files/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/x64/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/ARM64/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/x64/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/ARM64/*
+
+Saved/
+LocalBuilds/
+*.csproj.*
+.vs/*
+.vsconfig
+*.pdb
+*.suo
+*.opensdf
+*.sdf
+*.tmp
+*.mdb
+obj/
+*.vcxproj
+*.sln
+*-Debug.*
+FileOpenOrder/
+*.xcworkspace
+*.xcodeproj
+./Makefile
+./CMakeLists.txt
+.ue4dependencies
+Samples/*
+FeaturePacks/*
+Templates/*
+Engine/Documentation/*
+
+# Engine intermediates
+Engine/Intermediate/*
+Intermediate/
+
+# Intermediate folders for programs should not be checked in
+Engine\Programs\*\Intermediate\*
+
+# Intermediate folders created for various C# programs
+Engine\Source\Programs\*\obj\*
+
+# Saved folders for programs should not be checked in
+Engine\Programs\*\Saved\*
+Engine\Programs\UnrealBuildTool\*
+
+# Derived data cache should never be checked in
+Engine/DerivedDataCache/*
+
+# Ignore any build receipts
+Engine/Build/Receipts/*
+
+# Ignore personal workspace vars
+p4config.txt
+
+# Ignore Unix backup files
+*~
+
+# Ignore Mac desktop services store files
+.DS_Store
+
+# Ignore crash reports
+crashinfo--*
+
+# Ignore linux project files
+*.user
+*.pro
+*.pri
+*.kdev4
+
+# Obj-C/Swift specific
+*.hmap
+*.ipa
+*.dSYM.zip
+*.dSYM
+
+# Ignore documentation generated for C# tools
+Engine/Binaries/DotNET/UnrealBuildTool.xml
+Engine/Binaries/DotNET/AutomationScripts/BuildGraph.Automation.xml
+
+# Ignore version files in the Engine/Binaries directory created by UBT
+/Engine/Binaries/**/*.version
+
+# Ignore exp files in the the Engine/Binaries directory as they aren't C/C++ source files
+/Engine/Binaries/**/*.exp
+
+# Ignore Swarm local save files
+Engine/Binaries/DotNET/SwarmAgent.DeveloperOptions.xml
+Engine/Binaries/DotNET/SwarmAgent.Options.xml
+
+# Intermediary Files
+*.target.xml
+*.exe.config
+*.exe.manifest
+
+# Ignore project-specific files
+*/Build/Receipts/*
+*/DerivedDataCache/*
+*/Binaries/*-Shipping.*
+*/Intermediate/*
+
+*/Logs/*
```

### Comparing `unknown-cli-0.9.3/unknowncli/set_registry_keys.py` & `unknown-cli-0.9.4/unknowncli/set_registry_keys.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.3/unknowncli/set_url_handler.py` & `unknown-cli-0.9.4/unknowncli/set_url_handler.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.3/unknowncli/utils.py` & `unknown-cli-0.9.4/unknowncli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,9 +347,9 @@
         if not val:
             raise
     except:
         add_key = True
     
     if add_key:
         path = Path(__file__).parent / "set_url_handler.py"
-        cmd = f"{sys.executable} {path.resolve()} {exe}"
+        cmd = f"{sys.executable} \"{path.resolve()}\" {exe}"
         call(cmd)
```

