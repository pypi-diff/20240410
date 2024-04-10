# Comparing `tmp/DLMS_SPODES_communications-1.2.3.tar.gz` & `tmp/DLMS_SPODES_communications-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_communications-1.2.3.tar", last modified: Wed Feb 21 12:58:32 2024, max compression
+gzip compressed data, was "DLMS_SPODES_communications-1.2.4.tar", last modified: Wed Apr 10 06:46:47 2024, max compression
```

## Comparing `DLMS_SPODES_communications-1.2.3.tar` & `DLMS_SPODES_communications-1.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-02-21 12:58:32.527433 DLMS_SPODES_communications-1.2.3/
--rw-rw-rw-   0        0        0      527 2024-02-21 12:58:32.526468 DLMS_SPODES_communications-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       61 2024-01-18 10:40:20.000000 DLMS_SPODES_communications-1.2.3/README.md
--rw-rw-rw-   0        0        0      851 2024-02-21 12:26:51.000000 DLMS_SPODES_communications-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-21 12:58:32.527433 DLMS_SPODES_communications-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0       43 2024-01-19 07:53:50.000000 DLMS_SPODES_communications-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:58:32.457359 DLMS_SPODES_communications-1.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-02-21 12:58:32.509433 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/
--rw-rw-rw-   0        0        0      572 2024-02-14 09:26:43.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/__init__.py
--rw-rw-rw-   0        0        0     2769 2024-02-15 10:30:30.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/base.py
--rw-rw-rw-   0        0        0    11579 2024-01-19 05:28:12.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/ble.py
--rw-rw-rw-   0        0        0     3094 2024-02-14 09:17:34.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/network.py
--rw-rw-rw-   0        0        0     4205 2024-02-21 12:25:04.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/serial_port.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:58:32.520434 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/
--rw-rw-rw-   0        0        0      527 2024-02-21 12:58:32.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2024-02-21 12:58:32.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-21 12:58:32.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-02-21 12:58:32.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2024-02-21 12:58:32.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-02-21 12:58:32.000000 DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-21 12:58:32.524470 DLMS_SPODES_communications-1.2.3/test/
--rw-rw-rw-   0        0        0     1035 2024-02-14 09:19:03.000000 DLMS_SPODES_communications-1.2.3/test/test_Network.py
--rw-rw-rw-   0        0        0      982 2024-02-14 09:18:59.000000 DLMS_SPODES_communications-1.2.3/test/test_Serial.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.809666 DLMS_SPODES_communications-1.2.4/
+-rw-rw-rw-   0        0        0      527 2024-04-10 06:46:47.808664 DLMS_SPODES_communications-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2024-01-18 10:40:20.000000 DLMS_SPODES_communications-1.2.4/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-10 06:41:28.000000 DLMS_SPODES_communications-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 06:46:47.810667 DLMS_SPODES_communications-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-01-19 07:53:50.000000 DLMS_SPODES_communications-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.770662 DLMS_SPODES_communications-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.788663 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/
+-rw-rw-rw-   0        0        0      572 2024-02-14 09:26:43.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/__init__.py
+-rw-rw-rw-   0        0        0     2769 2024-04-10 06:04:37.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/base.py
+-rw-rw-rw-   0        0        0    11579 2024-01-19 05:28:12.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/ble.py
+-rw-rw-rw-   0        0        0     3094 2024-02-14 09:17:34.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/network.py
+-rw-rw-rw-   0        0        0     4366 2024-04-10 06:11:51.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/serial_port.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.802665 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.806663 DLMS_SPODES_communications-1.2.4/test/
+-rw-rw-rw-   0        0        0     1035 2024-02-14 09:19:03.000000 DLMS_SPODES_communications-1.2.4/test/test_Network.py
+-rw-rw-rw-   0        0        0     1695 2024-04-10 06:09:40.000000 DLMS_SPODES_communications-1.2.4/test/test_Serial.py
```

### Comparing `DLMS_SPODES_communications-1.2.3/PKG-INFO` & `DLMS_SPODES_communications-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_communications
-Version: 1.2.3
+Version: 1.2.4
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSSPODEScommunication_prj
 Keywords: dlms,drivers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_SPODES_communications-1.2.3/pyproject.toml` & `DLMS_SPODES_communications-1.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_communications"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "bleak==0.20.2",
     "netaddr>=0.8.0",
     "pyserial>=3.5",
```

### Comparing `DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/__init__.py` & `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/base.py` & `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/base.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/ble.py` & `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/ble.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/network.py` & `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/network.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications/serial_port.py` & `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/serial_port.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from typing import Any
 from serial_asyncio import open_serial_connection
 import serial
 from serial import Serial
 from .base import Base, StreamBase
 
 BAUD_RATE: int = 9600
@@ -127,7 +128,11 @@
         return F"{self.__class__.__name__}({', '.join(params)})"
 
     async def open(self):
         """ coroutine start """
         self.reader, self.writer = await open_serial_connection(
             url=self.port,
             baudrate=self.baudrate)
+
+    async def close(self):
+        await asyncio.sleep(.1)  # need delay before close writer
+        await super(AsyncSerial, self).close()
```

### Comparing `DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/PKG-INFO` & `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-communications
-Version: 1.2.3
+Version: 1.2.4
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSSPODEScommunication_prj
 Keywords: dlms,drivers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_SPODES_communications-1.2.3/src/DLMS_SPODES_communications.egg-info/SOURCES.txt` & `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.3/test/test_Network.py` & `DLMS_SPODES_communications-1.2.4/test/test_Network.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.3/test/test_Serial.py` & `DLMS_SPODES_communications-1.2.4/test/test_Serial.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,17 +16,38 @@
         print(F"{buf.hex(' ')=}")
         driver.close()
 
     def test_AsyncSerial(self):
         async def main(d: AsyncSerial):
             await d.open()
             print(F"{driver.is_open()=}")
-            data = bytes.fromhex("7E A0 07 03 21 93 0F 01 7E")
+            data = bytes.fromhex("7E A0 07 05 21 93 0F 01 7E")
             await driver.send(data)
             buf = bytearray()
             await driver.receive(buf)
             print(F"{buf.hex(' ')=}")
             await d.close()
 
         driver = AsyncSerial(
-            port="COM3")
+            port="COM13",
+            inactivity_timeout=2)
+        asyncio.run(main(driver))
+
+    def test_AsyncSerial_without_recv(self):
+        async def main(d: AsyncSerial):
+            await d.open()
+            print(F"{driver.is_open()=}")
+            data = bytes.fromhex("7E A0 07 05 21 93 0F 01 7E")
+            await driver.send(data)
+            await d.close()
+            print("1 end")
+            await d.open()
+            print(F"{driver.is_open()=}")
+            data = bytes.fromhex("7E A0 07 06 21 93 0F 01 7E")
+            await driver.send(data)
+            await d.close()
+            print("2 end")
+
+        driver = AsyncSerial(
+            port="COM13",
+            inactivity_timeout=2)
         asyncio.run(main(driver))
```

