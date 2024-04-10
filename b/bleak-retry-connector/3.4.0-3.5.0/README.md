# Comparing `tmp/bleak_retry_connector-3.4.0.tar.gz` & `tmp/bleak_retry_connector-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bleak_retry_connector-3.4.0.tar", max compression
+gzip compressed data, was "bleak_retry_connector-3.5.0.tar", max compression
```

## Comparing `bleak_retry_connector-3.4.0.tar` & `bleak_retry_connector-3.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/LICENSE
--rw-r--r--   0        0        0     3679 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/README.md
--rw-r--r--   0        0        0     2492 2024-01-01 18:31:34.845712 bleak_retry_connector-3.4.0/pyproject.toml
--rw-r--r--   0        0        0    18813 2024-01-01 18:31:34.821712 bleak_retry_connector-3.4.0/src/bleak_retry_connector/__init__.py
--rw-r--r--   0        0        0     2294 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/src/bleak_retry_connector/bleak_manager.py
--rw-r--r--   0        0        0    16386 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/src/bleak_retry_connector/bluez.py
--rw-r--r--   0        0        0      219 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/src/bleak_retry_connector/const.py
--rw-r--r--   0        0        0     1369 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/src/bleak_retry_connector/dbus.py
--rw-r--r--   0        0        0        0 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/src/bleak_retry_connector/py.typed
--rw-r--r--   0        0        0      280 2024-01-01 18:31:34.173710 bleak_retry_connector-3.4.0/src/bleak_retry_connector/util.py
--rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 bleak_retry_connector-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/LICENSE
+-rw-r--r--   0        0        0     3679 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/README.md
+-rw-r--r--   0        0        0     2492 2024-04-10 01:44:17.942871 bleak_retry_connector-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18813 2024-04-10 01:44:17.918871 bleak_retry_connector-3.5.0/src/bleak_retry_connector/__init__.py
+-rw-r--r--   0        0        0     2294 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/src/bleak_retry_connector/bleak_manager.py
+-rw-r--r--   0        0        0    16478 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/src/bleak_retry_connector/bluez.py
+-rw-r--r--   0        0        0      219 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/src/bleak_retry_connector/const.py
+-rw-r--r--   0        0        0     1369 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/src/bleak_retry_connector/dbus.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/src/bleak_retry_connector/py.typed
+-rw-r--r--   0        0        0      280 2024-04-10 01:44:17.198871 bleak_retry_connector-3.5.0/src/bleak_retry_connector/util.py
+-rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 bleak_retry_connector-3.5.0/PKG-INFO
```

### Comparing `bleak_retry_connector-3.4.0/LICENSE` & `bleak_retry_connector-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bleak_retry_connector-3.4.0/README.md` & `bleak_retry_connector-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bleak_retry_connector-3.4.0/pyproject.toml` & `bleak_retry_connector-3.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bleak-retry-connector"
-version = "3.4.0"
+version = "3.5.0"
 description = "A connector for Bleak Clients that handles transient connection failures"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bleak-retry-connector"
 documentation = "https://bleak-retry-connector.readthedocs.io"
 classifiers = [
```

### Comparing `bleak_retry_connector-3.4.0/src/bleak_retry_connector/__init__.py` & `bleak_retry_connector-3.5.0/src/bleak_retry_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "3.4.0"
+__version__ = "3.5.0"
 
 
 import asyncio
 import logging
 from collections.abc import Awaitable, Callable
 from typing import Any, ParamSpec, TypeVar
```

### Comparing `bleak_retry_connector-3.4.0/src/bleak_retry_connector/bleak_manager.py` & `bleak_retry_connector-3.5.0/src/bleak_retry_connector/bleak_manager.py`

 * *Files identical despite different names*

### Comparing `bleak_retry_connector-3.4.0/src/bleak_retry_connector/bluez.py` & `bleak_retry_connector-3.5.0/src/bleak_retry_connector/bluez.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,25 +286,26 @@
     if (
         not IS_LINUX
         or not isinstance(device.details, dict)
         or "path" not in device.details
     ):
         await asyncio.sleep(min_wait_time)
         return
+    device_path = device.details["path"]
     start = time.monotonic() if min_wait_time else 0
     try:
         if not (manager := await get_global_bluez_manager_with_timeout()):
             _LOGGER.debug(
                 "%s - %s: Failed to wait for disconnect because no manager",
                 device.name,
                 device.address,
             )
             return
         async with asyncio_timeout(DISCONNECT_TIMEOUT):
-            await manager._wait_condition(device.details["path"], "Connected", False)
+            await manager._wait_condition(device_path, "Connected", False)
         end = time.monotonic() if min_wait_time else 0
         waited = end - start
         _LOGGER.debug(
             "%s - %s: Waited %s seconds to disconnect",
             device.name,
             device.address,
             waited,
@@ -316,27 +317,29 @@
         #
         # In testing it was found that most of the CSR adapters
         # only support 5 slots and the broadcom only support 7 slots.
         #
         # When they run out of slots the device they are trying to
         # connect to disappears from the bus so we must backoff
         _LOGGER.debug(
-            "%s - %s: Device was removed from bus, waiting %s for it to re-appear: (%s) %s",
+            "%s - %s: Device was removed from bus at %s, waiting %s for it to re-appear: (%s) %s",
             device.name,
             device.address,
+            device_path,
             min_wait_time,
             type(ex),
             ex,
         )
         await wait_for_device_to_reappear(device, min_wait_time)
     except Exception:  # pylint: disable=broad-except
         _LOGGER.debug(
-            "%s - %s: Failed waiting for disconnect",
+            "%s - %s: Failed waiting for disconnect at %s",
             device.name,
             device.address,
+            device_path,
             exc_info=True,
         )
 
 
 async def get_device_by_adapter(address: str, adapter: str) -> BLEDevice | None:
     """Get the device by adapter and address."""
     if not IS_LINUX:
```

### Comparing `bleak_retry_connector-3.4.0/src/bleak_retry_connector/dbus.py` & `bleak_retry_connector-3.5.0/src/bleak_retry_connector/dbus.py`

 * *Files identical despite different names*

### Comparing `bleak_retry_connector-3.4.0/PKG-INFO` & `bleak_retry_connector-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bleak-retry-connector
-Version: 3.4.0
+Version: 3.5.0
 Summary: A connector for Bleak Clients that handles transient connection failures
 Home-page: https://github.com/bluetooth-devices/bleak-retry-connector
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bleak-retry-connector Version: 3.4.0 Summary: A
+Metadata-Version: 2.1 Name: bleak-retry-connector Version: 3.5.0 Summary: A
 connector for Bleak Clients that handles transient connection failures Home-
 page: https://github.com/bluetooth-devices/bleak-retry-connector License: MIT
 Author: J. Nick Koston Author-email: nick@koston.org Requires-Python:
 >=3.10,<3.13 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

