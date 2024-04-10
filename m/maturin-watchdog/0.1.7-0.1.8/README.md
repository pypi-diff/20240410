# Comparing `tmp/maturin_watchdog-0.1.7.tar.gz` & `tmp/maturin_watchdog-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.7.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.8.tar", max compression
```

## Comparing `maturin_watchdog-0.1.7.tar` & `maturin_watchdog-0.1.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.7/README.md
--rw-r--r--   0        0        0      529 2024-04-10 16:56:21.266952 maturin_watchdog-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2650 2024-04-10 16:55:30.633066 maturin_watchdog-0.1.7/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.8/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 16:58:34.855455 maturin_watchdog-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2722 2024-04-10 16:58:28.238385 maturin_watchdog-0.1.8/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.8/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.7/pyproject.toml` & `maturin_watchdog-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maturin-watchdog"
-version = "0.1.7"
+version = "0.1.8"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

### Comparing `maturin_watchdog-0.1.7/src/maturin_watchdog/plugin.py` & `maturin_watchdog-0.1.8/src/maturin_watchdog/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         command = event.command
         if not isinstance(command, EnvCommand):
             return
         
         io = event.io
 
         # Print the command to be executed
-        io.write_line(
-            "<info>Command to be executed:</info> {}".format(command))
+        io.write_line("<info>Command description:</info> {}".format(command.description))
+        io.write_line("<info>Command name:</info> {}".format(command.name))
        
         # Check if Rust code needs to be rebuilt
         if self._rust_code_needs_rebuild():
             io.write_line("Rust code needs to be rebuilt.")
             # self._rebuild_rust_code()
         else:
             io.write_line("Rust code is up to date.")
```
