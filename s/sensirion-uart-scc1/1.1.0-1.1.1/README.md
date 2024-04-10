# Comparing `tmp/sensirion_uart_scc1-1.1.0.tar.gz` & `tmp/sensirion_uart_scc1-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensirion_uart_scc1-1.1.0.tar", max compression
+gzip compressed data, was "sensirion_uart_scc1-1.1.1.tar", max compression
```

## Comparing `sensirion_uart_scc1-1.1.0.tar` & `sensirion_uart_scc1-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1499 2024-04-09 16:10:13.939882 sensirion_uart_scc1-1.1.0/LICENSE
--rw-r--r--   0        0        0     3436 2024-04-09 16:10:13.939882 sensirion_uart_scc1-1.1.0/README.md
--rw-r--r--   0        0        0      872 2024-04-09 16:10:13.939882 sensirion_uart_scc1-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       24 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/__init__.py
--rw-r--r--   0        0        0       24 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/__init__.py
--rw-r--r--   0        0        0     7543 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/scc1_slf3x.py
--rw-r--r--   0        0        0     3825 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/slf_common.py
--rw-r--r--   0        0        0       24 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/__init__.py
--rw-r--r--   0        0        0     2283 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/i2c_transceiver.py
--rw-r--r--   0        0        0      605 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/shdlc_transceiver.py
--rw-r--r--   0        0        0      459 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_exceptions.py
--rw-r--r--   0        0        0     1596 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_i2c_transceiver.py
--rw-r--r--   0        0        0     5295 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_shdlc_device.py
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 sensirion_uart_scc1-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1499 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3436 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/README.md
+-rw-r--r--   0        0        0      873 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/drivers/__init__.py
+-rw-r--r--   0        0        0     7543 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/drivers/scc1_slf3x.py
+-rw-r--r--   0        0        0     3825 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/drivers/slf_common.py
+-rw-r--r--   0        0        0       24 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/protocols/__init__.py
+-rw-r--r--   0        0        0     2283 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/protocols/i2c_transceiver.py
+-rw-r--r--   0        0        0      605 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/protocols/shdlc_transceiver.py
+-rw-r--r--   0        0        0      459 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/scc1_exceptions.py
+-rw-r--r--   0        0        0     1596 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/scc1_i2c_transceiver.py
+-rw-r--r--   0        0        0     5644 2024-04-10 09:04:34.218218 sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/scc1_shdlc_device.py
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 sensirion_uart_scc1-1.1.1/PKG-INFO
```

### Comparing `sensirion_uart_scc1-1.1.0/LICENSE` & `sensirion_uart_scc1-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.1.0/README.md` & `sensirion_uart_scc1-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.1.0/pyproject.toml` & `sensirion_uart_scc1-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensirion-uart-scc1"
-version = "1.1.0"
+version = "1.1.1"
 description = "Driver for Sensirion SCC1 USB cable"
 authors = ["Pascal Sachs"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
@@ -25,14 +25,15 @@
 addopts = "--cov=sensirion_uart_scc1 --cov-report term --cov-report lcov --junitxml=test-report.xml"
 markers = "needs_hardware"
 testpaths = [
 	"tests"
 ]
 
 
+
 [tool.poetry.group.docs] 
 optional = true 
 
 [tool.poetry.group.docs.dependencies] 
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
```

### Comparing `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/scc1_slf3x.py` & `sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/drivers/scc1_slf3x.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/slf_common.py` & `sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/drivers/slf_common.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/i2c_transceiver.py` & `sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/protocols/i2c_transceiver.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/shdlc_transceiver.py` & `sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/protocols/shdlc_transceiver.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_i2c_transceiver.py` & `sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/scc1_i2c_transceiver.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_shdlc_device.py` & `sensirion_uart_scc1-1.1.1/sensirion_uart_scc1/scc1_shdlc_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import logging
 from struct import unpack
-from typing import Optional, Iterable, Union
+from typing import Optional, Iterable, Union, List
 
 from packaging.version import Version
 from sensirion_shdlc_driver import ShdlcDevice, ShdlcConnection
 from sensirion_shdlc_driver.command import ShdlcCommand
 
 from sensirion_uart_scc1.protocols.i2c_transceiver import I2cTransceiver
 from sensirion_uart_scc1.scc1_i2c_transceiver import Scc1I2cTransceiver
@@ -26,81 +26,87 @@
         :param slave_address: The SHDLC slave address that is used by this device.
         """
         super().__init__(connection, slave_address)
         self._version = self.get_version()
         self._serial_number = self.get_serial_number()
         self._sensor_type = self.get_sensor_type()
         self._i2c_address = self.get_sensor_address()
-        self._connected_i2c_addresses = {}
+        self._connected_i2c_addresses: List[int] = []
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"SCC1-{self.serial_number}@{self.com_port}"
 
     @property
-    def com_port(self):
+    def com_port(self) -> str:
         return self.connection.port.description.split('@')[0]
 
     @property
     def serial_number(self) -> str:
         return self._serial_number
 
     @property
     def firmware_version(self) -> Version:
         return Version(str(self._version.firmware))
 
-    def perform_i2c_scan(self):
+    @property
+    def connected_i2c_addresses(self) -> List[int]:
+        """Returns the connected I2C addresses. You need to call find_chips to fill this attribute."""
+        return self._connected_i2c_addresses
+
+    def perform_i2c_scan(self) -> List[int]:
         """
         Looks for i2c devices within a certain range on a certain port
         :return: List of i2c addresses that responded to the scan
         """
         result = self.transceive(0x29, [0x01], timeout=0.025)
         return list(unpack('>{cnt}B'.format(cnt=len(result)), result))
 
-    def find_chips(self):
+    def find_chips(self) -> List[int]:
         """
         Looking for chips on all ports and sets the _connected_i2c_addresses attribute
-        :return: Llist of connected addresses
+        :return: List of connected addresses
         """
         self._connected_i2c_addresses = self.perform_i2c_scan()
         return self._connected_i2c_addresses
 
-    def get_sensor_type(self):
+    def get_sensor_type(self) -> Optional[int]:
         """
         :return: the configured sensor type
         """
         result = self.transceive(0x24, [], timeout=0.025)
         if result:
             return int(unpack('>B', result)[0])
         return None
 
-    def set_sensor_type(self, sensor_type):
+    def set_sensor_type(self, sensor_type: int):
         """
         Set sensor type
         0: Flow Sensor (SF04 based products)
         1: Humidity Sensor (SHTxx products)
         2: Flow Sensor (SF05 based products)
         3: Flow Sensor (SF06 based products) (Firmware ≥1.7)
+        4: Reserved
         :param sensor_type: One of the supported sensor types 0-4
 
         """
         if sensor_type not in range(5):
             raise ValueError('Sensor type not supported')
         self.transceive(0x24, [sensor_type], timeout=0.01)
         self._sensor_type = sensor_type
 
-    def get_sensor_address(self):
+    def get_sensor_address(self) -> Optional[int]:
         """
         :return: the configured i2c address
         """
         result = self.transceive(0x25, [], timeout=0.025)
         if result:
             return int(unpack('>B', result)[0])
         return None
 
-    def set_sensor_address(self, i2c_address):
+    def set_sensor_address(self, i2c_address: int) -> None:
         """
         Configure the sensors i2c address and write it to EEPROM
         :param i2c_address: the i2c address
         """
         if i2c_address not in range(128):
             raise ValueError('I2C address out of range. Address has to be within the range 0...127')
         self.transceive(0x25, [i2c_address], timeout=0.01)
```

### Comparing `sensirion_uart_scc1-1.1.0/PKG-INFO` & `sensirion_uart_scc1-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensirion-uart-scc1
-Version: 1.1.0
+Version: 1.1.1
 Summary: Driver for Sensirion SCC1 USB cable
 License: BSD-3-Clause
 Author: Pascal Sachs
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

