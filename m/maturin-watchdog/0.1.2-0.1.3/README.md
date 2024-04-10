# Comparing `tmp/maturin_watchdog-0.1.2.tar.gz` & `tmp/maturin_watchdog-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.2.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.3.tar", max compression
```

## Comparing `maturin_watchdog-0.1.2.tar` & `maturin_watchdog-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.2/README.md
--rw-r--r--   0        0        0      529 2024-04-10 16:26:42.020243 maturin_watchdog-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1105 2024-04-10 16:20:11.085950 maturin_watchdog-0.1.2/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.3/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 16:28:54.546372 maturin_watchdog-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1152 2024-04-10 16:28:35.354602 maturin_watchdog-0.1.3/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.3/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.2/pyproject.toml` & `maturin_watchdog-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maturin-watchdog"
-version = "0.1.2"
+version = "0.1.3"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

### Comparing `maturin_watchdog-0.1.2/src/maturin_watchdog/plugin.py` & `maturin_watchdog-0.1.3/src/maturin_watchdog/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,14 @@
         dispatcher: EventDispatcher
     ) -> None:
         command = event.command
         if not isinstance(command, EnvCommand):
             return
 
         io = event.io
-
+        print("Loading environment variables.")
         if io.is_debug():
             io.write_line(
                 "<debug>Loading environment variables.</debug>"
             )
 
         load_dotenv()
```

