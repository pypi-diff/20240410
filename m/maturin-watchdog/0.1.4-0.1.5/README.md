# Comparing `tmp/maturin_watchdog-0.1.4.tar.gz` & `tmp/maturin_watchdog-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.4.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.5.tar", max compression
```

## Comparing `maturin_watchdog-0.1.4.tar` & `maturin_watchdog-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.4/README.md
--rw-r--r--   0        0        0      529 2024-04-10 16:33:22.078838 maturin_watchdog-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2447 2024-04-10 16:33:14.285661 maturin_watchdog-0.1.4/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.5/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 16:39:59.428658 maturin_watchdog-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2478 2024-04-10 16:39:48.303760 maturin_watchdog-0.1.5/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.5/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.4/pyproject.toml` & `maturin_watchdog-0.1.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maturin-watchdog"
-version = "0.1.4"
+version = "0.1.5"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

### Comparing `maturin_watchdog-0.1.4/src/maturin_watchdog/plugin.py` & `maturin_watchdog-0.1.5/src/maturin_watchdog/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         event: ConsoleCommandEvent,
         event_name: str,
         dispatcher: EventDispatcher
     ) -> None:
         command = event.command
         if not isinstance(command, EnvCommand):
             return
-
+        print(command)
         # Check if Rust code needs to be rebuilt
         if self._rust_code_needs_rebuild():
             print("Rust code needs to be rebuilt.")
             self._rebuild_rust_code()
         else:
             print("Rust code is up to date.")
 
@@ -39,15 +39,15 @@
         """
         Check if Rust code needs to be rebuilt by comparing
         timestamps of source files and compiled binaries.
         """
         # Define paths to Rust source files
         rust_src_dir = Path("src")
         rust_src_files = list(rust_src_dir.glob("*.rs"))
-        
+
         # Check if there are no Rust source files
         if not rust_src_files:
             return False  # No Rust code to rebuild
 
         # Check if the target directory exists
         target_dir = Path("target")
         if not target_dir.exists():
@@ -63,8 +63,8 @@
         return False  # No need to rebuild Rust code
 
     def _rebuild_rust_code(self):
         """
         Rebuild Rust code using cargo.
         """
         print("Rebuilding Rust code.")
-        subprocess.run(["cargo", "build"])  # Assuming cargo is in PATH
+        subprocess.run(["maturin", "develop", "--release"])  # Assuming cargo is in PATH
```

