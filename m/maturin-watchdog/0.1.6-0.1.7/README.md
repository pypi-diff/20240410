# Comparing `tmp/maturin_watchdog-0.1.6.tar.gz` & `tmp/maturin_watchdog-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.6.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.7.tar", max compression
```

## Comparing `maturin_watchdog-0.1.6.tar` & `maturin_watchdog-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.6/README.md
--rw-r--r--   0        0        0      529 2024-04-10 16:53:15.365288 maturin_watchdog-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2587 2024-04-10 16:53:07.206726 maturin_watchdog-0.1.6/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.7/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 16:56:21.266952 maturin_watchdog-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2650 2024-04-10 16:55:30.633066 maturin_watchdog-0.1.7/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.7/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.6/pyproject.toml` & `maturin_watchdog-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maturin-watchdog"
-version = "0.1.6"
+version = "0.1.7"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

### Comparing `maturin_watchdog-0.1.6/src/maturin_watchdog/plugin.py` & `maturin_watchdog-0.1.7/src/maturin_watchdog/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,23 +23,27 @@
         event: ConsoleCommandEvent,
         event_name: str,
         dispatcher: EventDispatcher
     ) -> None:
         command = event.command
         if not isinstance(command, EnvCommand):
             return
-        print("Commands",command.commands)
-        print("Arguments",command.arguments)
-        print("Options", command.options)
+        
+        io = event.io
+
+        # Print the command to be executed
+        io.write_line(
+            "<info>Command to be executed:</info> {}".format(command))
+       
         # Check if Rust code needs to be rebuilt
         if self._rust_code_needs_rebuild():
-            print("Rust code needs to be rebuilt.")
+            io.write_line("Rust code needs to be rebuilt.")
             # self._rebuild_rust_code()
         else:
-            print("Rust code is up to date.")
+            io.write_line("Rust code is up to date.")
 
     def _rust_code_needs_rebuild(self) -> bool:
         """
         Check if Rust code needs to be rebuilt by comparing
         timestamps of source files and compiled binaries.
         """
         # Define paths to Rust source files
```

