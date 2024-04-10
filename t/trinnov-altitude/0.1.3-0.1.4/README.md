# Comparing `tmp/trinnov-altitude-0.1.3.tar.gz` & `tmp/trinnov-altitude-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.3.tar", last modified: Wed Apr 10 00:48:14 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.4.tar", last modified: Wed Apr 10 00:58:01 2024, max compression
```

## Comparing `trinnov-altitude-0.1.3.tar` & `trinnov-altitude-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:48:14.589282 trinnov-altitude-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-10 00:48:14.589282 trinnov-altitude-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-10 00:48:14.589282 trinnov-altitude-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:48:14.585282 trinnov-altitude-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:48:14.585282 trinnov-altitude-0.1.3/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-10 00:48:03.000000 trinnov-altitude-0.1.3/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:48:14.585282 trinnov-altitude-0.1.3/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-10 00:48:14.000000 trinnov-altitude-0.1.3/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-10 00:48:14.000000 trinnov-altitude-0.1.3/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:48:14.000000 trinnov-altitude-0.1.3/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 00:48:14.000000 trinnov-altitude-0.1.3/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.868435 trinnov-altitude-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.3/LICENSE` & `trinnov-altitude-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.3/README.md` & `trinnov-altitude-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.3/setup.cfg` & `trinnov-altitude-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = trinnov-altitude
 version = attr: trinnov_altitude.__version__
 description = "Python client for interfacing with the Trinnov Altitude processor."
-long_description = file: README.rst
+long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/binarylogic/py-trinnov-altitude
 author = Ben Johnson
 author_email = ben@binarylogic.com
 licence = Apache 2.0
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `trinnov-altitude-0.1.3/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.4/tests/test_trinnov_altitude.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.3/trinnov_altitude/const.py` & `trinnov-altitude-0.1.4/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.3/trinnov_altitude/exceptions.py` & `trinnov-altitude-0.1.4/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.3/trinnov_altitude/messages.py` & `trinnov-altitude-0.1.4/trinnov_altitude/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 
 
-def message_factory(message) -> Message | None:
+def message_factory(message) -> Message | None:  # noqa: C901
     if match := re.match(r"^AUDIOSYNC\s(0|1)", message):
         state = bool(int(match.group(1)))
         return AudiosyncMessage(state)
     elif match := re.match(r"^BYPASS\s(0|1)", message):
         state = bool(int(match.group(1)))
         return BypassMessage(state)
     elif match := re.match(r"^DIM\s(-?\d+)", message):
@@ -19,15 +19,15 @@
     elif match := re.match(r"^LABEL\s(-?\d+): (.*)", message):
         index = int(match.group(1))
         name = match.group(2)
         return PresetMessage(index, name)
     elif match := re.match(r"^LABELS_CLEAR", message):
         return PresetsClearMessage()
     elif match := re.match(r"^MUTE\s(0|1)", message):
-        mute = bool(int(match.group(1)))
+        state = bool(int(match.group(1)))
         return MuteMessage(state)
     elif match := re.match(r"^OK", message):
         return OKMessage()
     elif match := re.match(r"^PROFILE\s(-?\d+): (.*)", message):
         index = int(match.group(1))
         name = match.group(2)
         return SourceMessage(index, name)
```

### Comparing `trinnov-altitude-0.1.3/trinnov_altitude/mocks.py` & `trinnov-altitude-0.1.4/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.3/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.4/trinnov_altitude/trinnov_altitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             self._response_handler_task.cancel()
             try:
                 await self._response_handler_task
             except asyncio.CancelledError:
                 pass
             self._response_handler_task = None
 
-        await self._send(f"bye", timeout)
+        await self._send("bye", timeout)
         self._writer.close()
         await asyncio.wait_for(self._writer.wait_closed(), timeout)
         self._reader = None
         self._writer = None
 
     def register_callback(self, callback: Callable[[messages.Message], None]):
         self._callback = callback
@@ -317,15 +317,15 @@
             message += "\n"
 
         message_bytes = message.encode(self.ENCODING)
         self._writer.write(message_bytes)
         await asyncio.wait_for(self._writer.drain(), timeout=timeout)
         self.logger.debug(f"Sent to Altitude: {message.rstrip()}")
 
-    async def _sync(self):
+    async def _sync(self):  # noqa: C901
         """
         Sync internal state
 
         Receives all broadcasted messages from the proessor and syncs the
         internal state.
         """
         while True:
@@ -339,15 +339,15 @@
                 self.audiosync = message.state
             elif isinstance(message, messages.BypassMessage):
                 self.bypass = message.state
             elif isinstance(message, messages.DimMessage):
                 self.dim = message.state
             elif isinstance(message, messages.ErrorMessage):
                 self.logger.error(
-                    f"Trinnov Altitude responsed with error: {error.error}"
+                    f"Trinnov Altitude responsed with error: {message.error}"
                 )
             elif isinstance(message, messages.PresetMessage):
                 self.presets[message.index] = message.name
             elif isinstance(message, messages.PresetsClearMessage):
                 self.presets = {}
             elif isinstance(message, messages.MuteMessage):
                 self.mute = message.state
```

