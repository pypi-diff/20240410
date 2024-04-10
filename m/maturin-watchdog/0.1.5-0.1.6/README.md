# Comparing `tmp/maturin_watchdog-0.1.5.tar.gz` & `tmp/maturin_watchdog-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.5.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.6.tar", max compression
```

## Comparing `maturin_watchdog-0.1.5.tar` & `maturin_watchdog-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.5/README.md
--rw-r--r--   0        0        0      529 2024-04-10 16:39:59.428658 maturin_watchdog-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2478 2024-04-10 16:39:48.303760 maturin_watchdog-0.1.5/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.6/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 16:53:15.365288 maturin_watchdog-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2587 2024-04-10 16:53:07.206726 maturin_watchdog-0.1.6/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.6/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.5/pyproject.toml` & `maturin_watchdog-0.1.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maturin-watchdog"
-version = "0.1.5"
+version = "0.1.6"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

### Comparing `maturin_watchdog-0.1.5/src/maturin_watchdog/plugin.py` & `maturin_watchdog-0.1.6/src/maturin_watchdog/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,19 +23,21 @@
         event: ConsoleCommandEvent,
         event_name: str,
         dispatcher: EventDispatcher
     ) -> None:
         command = event.command
         if not isinstance(command, EnvCommand):
             return
-        print(command)
+        print("Commands",command.commands)
+        print("Arguments",command.arguments)
+        print("Options", command.options)
         # Check if Rust code needs to be rebuilt
         if self._rust_code_needs_rebuild():
             print("Rust code needs to be rebuilt.")
-            self._rebuild_rust_code()
+            # self._rebuild_rust_code()
         else:
             print("Rust code is up to date.")
 
     def _rust_code_needs_rebuild(self) -> bool:
         """
         Check if Rust code needs to be rebuilt by comparing
         timestamps of source files and compiled binaries.
```

