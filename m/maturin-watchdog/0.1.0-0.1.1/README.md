# Comparing `tmp/maturin_watchdog-0.1.0.tar.gz` & `tmp/maturin_watchdog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.0.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.1.tar", max compression
```

## Comparing `maturin_watchdog-0.1.0.tar` & `maturin_watchdog-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.0/README.md
--rw-r--r--   0        0        0      523 2024-04-10 16:14:55.204162 maturin_watchdog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1112 2024-04-10 16:15:09.804148 maturin_watchdog-0.1.0/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.1/README.md
+-rw-r--r--   0        0        0      421 2024-04-10 16:23:14.083128 maturin_watchdog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1105 2024-04-10 16:20:11.085950 maturin_watchdog-0.1.1/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.1/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.0/src/maturin_watchdog/plugin.py` & `maturin_watchdog-0.1.1/src/maturin_watchdog/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cleo.events.event_dispatcher import EventDispatcher
 from dotenv import load_dotenv
 from poetry.console.application import Application
 from poetry.console.commands.env_command import EnvCommand
 from poetry.plugins.application_plugin import ApplicationPlugin
 
 
-class MyApplicationPlugin(ApplicationPlugin):
+class PoetryPlugin(ApplicationPlugin):
     def activate(self, application: Application):
         application.event_dispatcher.add_listener(
             COMMAND, self.load_dotenv
         )
 
     def load_dotenv(
         self,
```

