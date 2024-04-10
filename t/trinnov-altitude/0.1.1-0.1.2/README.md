# Comparing `tmp/trinnov-altitude-0.1.1.tar.gz` & `tmp/trinnov-altitude-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.1.tar", last modified: Tue Apr  9 16:52:34 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.2.tar", last modified: Tue Apr  9 20:28:02 2024, max compression
```

## Comparing `trinnov-altitude-0.1.1.tar` & `trinnov-altitude-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.755650 trinnov-altitude-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.755650 trinnov-altitude-0.1.1/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:02.302408 trinnov-altitude-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 20:28:02.302408 trinnov-altitude-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 20:28:02.302408 trinnov-altitude-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:02.302408 trinnov-altitude-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:02.302408 trinnov-altitude-0.1.2/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-09 20:27:58.000000 trinnov-altitude-0.1.2/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:02.302408 trinnov-altitude-0.1.2/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 20:28:02.000000 trinnov-altitude-0.1.2/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 20:28:02.000000 trinnov-altitude-0.1.2/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:28:02.000000 trinnov-altitude-0.1.2/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 20:28:02.000000 trinnov-altitude-0.1.2/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.1/LICENSE` & `trinnov-altitude-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.1/PKG-INFO` & `trinnov-altitude-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.1
+Version: 0.1.2
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinnov-altitude-0.1.1/README.md` & `trinnov-altitude-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.1/setup.cfg` & `trinnov-altitude-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.1/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.2/tests/test_trinnov_altitude.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,26 +34,47 @@
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
     await client.connect()
     assert client.connected() is True
     await client.disconnect()
 
 
 @pytest.mark.asyncio
+async def test_callback(mock_server):
+    client = TrinnovAltitude(host="localhost", port=mock_server.port)
+
+    def _update(event: str):
+        client._last_event = event  # type: ignore
+
+    client.register_callback(_update)
+    await client.connect()
+
+    # Wait for sync task
+    await asyncio.sleep(2)
+    await client.disconnect()
+
+    assert client._last_event == "OK"  # type: ignore
+
+
+@pytest.mark.asyncio
 async def test_set_volume(mock_server):
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
     await client.connect()
     await client.set_volume(-46)
-    await asyncio.sleep(0.1)
-    await client.sync()
+
+    # Wait for sync task
+    await asyncio.sleep(0.5)
+
     assert client.volume == -46.0
     await client.disconnect()
 
 
 @pytest.mark.asyncio
 async def test_adjust_volume(mock_server):
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
     await client.connect()
     await client.adjust_volume(2)
-    await asyncio.sleep(0.1)
-    await client.sync()
+
+    # Wait for sync task
+    await asyncio.sleep(0.5)
+
     assert client.volume == -38.0
     await client.disconnect()
```

### Comparing `trinnov-altitude-0.1.1/trinnov_altitude/exceptions.py` & `trinnov-altitude-0.1.2/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.1/trinnov_altitude/mocks.py` & `trinnov-altitude-0.1.2/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.1/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.2/trinnov_altitude/trinnov_altitude.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Implements the Trinnov Altitude processor automation protocol over TCP/IP
 """
 
 import asyncio
+from collections.abc import Callable
 import logging
 import re
 from trinnov_altitude import exceptions
 
 
 class TrinnovAltitude:
     """
@@ -36,23 +37,25 @@
         self.host = host
         self.port = port
         self.client_id = client_id
         self.timeout = timeout
         self.logger = logger
 
         # State
-        self.dim = None
-        self.id = None
-        self.mute = None
-        self.version = None
-        self.volume = None
+        self.dim: bool | None = None
+        self.id: str | None = None
+        self.mute: bool | None = None
+        self.version: str | None = None
+        self.volume: float | None = None
 
         # Utility
-        self._reader = None
-        self._writer = None
+        self._callback: Callable | None = None
+        self._reader: asyncio.StreamReader | None = None
+        self._response_handler_task: asyncio.Task | None = None
+        self._writer: asyncio.StreamWriter | None = None
 
     # --------------------------
     # Connection
     # --------------------------
 
     async def connect(self, timeout=USE_DEFAULT_TIMEOUT):
         """Initiates connection to the processor"""
@@ -66,60 +69,45 @@
                 asyncio.open_connection(self.host, self.port), timeout
             )
         except asyncio.TimeoutError:
             raise exceptions.ConnectionTimeoutError
         except Exception as e:
             raise exceptions.ConnectionFailedError(e)
 
+        self._response_handler_task = asyncio.create_task(self._sync())
+
         await self._send(f"id {self.client_id}", timeout)
 
     def connected(self):
         return self._reader is not None and self._writer is not None
 
-    async def sync(self, timeout=USE_DEFAULT_TIMEOUT):
-        """
-        Sync internal state
-
-        Receives all broadcasted messages from the proessor and syncs the
-        internal state.
-        """
-        while True:
-            message = await self._receive(timeout)
-            if message is None:
-                break
-
-            if match := re.match(r"^DIM\s(-?\d+)", message):
-                self.dim = bool(int(match.group(1)))
-            elif match := re.match(r"^ERROR: (.*)", message):
-                error = match.group(1)
-                self.logger.error(f"Trinnov Altitude responses with error: {error}")
-            elif match := re.match(r"^MUTE\s(0|1)", message):
-                self.mute = bool(int(match.group(1)))
-            elif match := re.match(r"^VOLUME\s(-?\d+(\.\d+)?)", message):
-                self.volume = float(match.group(1))
-            elif match := re.match(
-                r"^Welcome on Trinnov Optimizer \(Version (\S+), ID (\d+)\)",
-                message,
-            ):
-                self.version = match.group(1)
-                self.id = match.group(2)
-
     async def disconnect(self, timeout=USE_DEFAULT_TIMEOUT):
         """Closes the connection to the processor"""
         if self._writer is None:
             return
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
 
+        if self._response_handler_task:
+            self._response_handler_task.cancel()
+            try:
+                await self._response_handler_task
+            except asyncio.CancelledError:
+                pass
+            self._response_handler_task = None
+
         self._writer.close()
         await asyncio.wait_for(self._writer.wait_closed(), timeout)
         self._reader = None
         self._writer = None
 
+    def register_callback(self, callback: Callable):
+        self._callback = callback
+
     # --------------------------
     # Commands
     # --------------------------
 
     async def set_volume(self, db: int, timeout=USE_DEFAULT_TIMEOUT):
         """
         Set the master volume to an absolute value.
@@ -180,7 +168,38 @@
         if not message.endswith("\n"):
             message += "\n"
 
         message_bytes = message.encode(self.ENCODING)
         self._writer.write(message_bytes)
         await asyncio.wait_for(self._writer.drain(), timeout=timeout)
         self.logger.debug(f"Sent to Altitude: {message.rstrip()}")
+
+    async def _sync(self):
+        """
+        Sync internal state
+
+        Receives all broadcasted messages from the proessor and syncs the
+        internal state.
+        """
+        while True:
+            message = await self._receive(None)
+            if message is None:
+                break
+
+            if match := re.match(r"^DIM\s(-?\d+)", message):
+                self.dim = bool(int(match.group(1)))
+            elif match := re.match(r"^ERROR: (.*)", message):
+                error = match.group(1)
+                self.logger.error(f"Trinnov Altitude responses with error: {error}")
+            elif match := re.match(r"^MUTE\s(0|1)", message):
+                self.mute = bool(int(match.group(1)))
+            elif match := re.match(r"^VOLUME\s(-?\d+(\.\d+)?)", message):
+                self.volume = float(match.group(1))
+            elif match := re.match(
+                r"^Welcome on Trinnov Optimizer \(Version (\S+), ID (\d+)\)",
+                message,
+            ):
+                self.version = match.group(1)
+                self.id = match.group(2)
+
+            if self._callback is not None:
+                self._callback(message)
```

### Comparing `trinnov-altitude-0.1.1/trinnov_altitude.egg-info/PKG-INFO` & `trinnov-altitude-0.1.2/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.1
+Version: 0.1.2
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

