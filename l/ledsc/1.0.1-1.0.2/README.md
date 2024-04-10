# Comparing `tmp/ledsc-1.0.1.tar.gz` & `tmp/ledsc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledsc-1.0.1.tar", last modified: Fri Mar 15 08:08:18 2024, max compression
+gzip compressed data, was "ledsc-1.0.2.tar", last modified: Wed Apr 10 21:31:14 2024, max compression
```

## Comparing `ledsc-1.0.1.tar` & `ledsc-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hell      (1000) hell      (1000)        0 2024-03-15 08:08:18.221100 ledsc-1.0.1/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-03-15 08:08:18.221100 ledsc-1.0.1/PKG-INFO
--rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.1/README.md
-drwxr-xr-x   0 hell      (1000) hell      (1000)        0 2024-03-15 08:08:18.217100 ledsc-1.0.1/ledsc/
--rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-03-15 08:08:09.000000 ledsc-1.0.1/ledsc/__init__.py
--rw-r--r--   0 hell      (1000) hell      (1000)     7253 2024-03-15 08:08:09.000000 ledsc-1.0.1/ledsc/ledsc.py
-drwxr-xr-x   0 hell      (1000) hell      (1000)        0 2024-03-15 08:08:18.221100 ledsc-1.0.1/ledsc.egg-info/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-03-15 08:08:18.000000 ledsc-1.0.1/ledsc.egg-info/PKG-INFO
--rw-r--r--   0 hell      (1000) hell      (1000)      201 2024-03-15 08:08:18.000000 ledsc-1.0.1/ledsc.egg-info/SOURCES.txt
--rw-r--r--   0 hell      (1000) hell      (1000)        1 2024-03-15 08:08:18.000000 ledsc-1.0.1/ledsc.egg-info/dependency_links.txt
--rw-r--r--   0 hell      (1000) hell      (1000)       30 2024-03-15 08:08:18.000000 ledsc-1.0.1/ledsc.egg-info/requires.txt
--rw-r--r--   0 hell      (1000) hell      (1000)        6 2024-03-15 08:08:18.000000 ledsc-1.0.1/ledsc.egg-info/top_level.txt
--rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-03-15 08:08:09.000000 ledsc-1.0.1/pyproject.toml
--rw-r--r--   0 hell      (1000) hell      (1000)       38 2024-03-15 08:08:18.221100 ledsc-1.0.1/setup.cfg
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:31:14.465274 ledsc-1.0.2/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:31:14.465274 ledsc-1.0.2/PKG-INFO
+-rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.2/README.md
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:31:14.465274 ledsc-1.0.2/ledsc/
+-rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-03-15 08:08:09.000000 ledsc-1.0.2/ledsc/__init__.py
+-rw-r--r--   0 hell      (1000) hell      (1000)     7257 2024-04-10 21:30:26.000000 ledsc-1.0.2/ledsc/ledsc.py
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:31:14.465274 ledsc-1.0.2/ledsc.egg-info/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)      201 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/SOURCES.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/dependency_links.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       30 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/requires.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        6 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/top_level.txt
+-rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-04-10 21:30:26.000000 ledsc-1.0.2/pyproject.toml
+-rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-04-10 21:31:14.465274 ledsc-1.0.2/setup.cfg
```

### Comparing `ledsc-1.0.1/PKG-INFO` & `ledsc-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ledsc-1.0.1/README.md` & `ledsc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ledsc-1.0.1/ledsc/ledsc.py` & `ledsc-1.0.2/ledsc/ledsc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from enum import Enum
-from typing import List
+from typing import List, Callable
 
 from pymodbus.client import ModbusSerialClient
+from pymodbus.pdu import ModbusResponse
 
 
 class REG(Enum):
     LED_R = 0
     LED_G = 1
     LED_B = 2
     LED_W = 3
@@ -44,80 +45,89 @@
 
     def __response_check(self, resp):
         if self.slave_id != 0 and issubclass(type(resp), Exception):
             raise resp
 
     def read_register(self, address: int, count: int = 1):
         """
-        :param count: pocet ctenych registru
-        :param address: adresa modbus registru
+        :param count: number of bytes to read
+        :param address: address to read
         """
         if self.slave_id == 0:
             raise ValueError(f"Reading values is not available in BROADCAST mode!")
 
         resp = self.client.read_holding_registers(address=address, slave=self.slave_id, count=count)
         self.__response_check(resp)
         resp = resp.registers[0] if len(resp.registers) == 1 else resp.registers
         return resp
 
-    def write_register(self, address: int, value: int):
-        """
-        :param address: adresa modbus registru
-        :param value: zapisovana hodnota
-        """
-        timeout = self.client.comm_params.timeout_connect
-        if self.slave_id == 0:
+    def __write(self, func: Callable[[], ModbusResponse]):
+        is_broadcast = self.slave_id == 0
+        if is_broadcast:
+            timeout = self.client.comm_params.timeout_connect
             self.client.close()
             self.client.comm_params.timeout_connect = 0.000001
 
-        logging.debug(f"LedController: Writing register ({self.slave_id}): {address}={value}")
-        resp = self.client.write_register(address=address, slave=self.slave_id, value=value)
+        resp = func()
 
-        if self.slave_id == 0:
-            self.client.comm_params.timeout_connect = timeout
+        if is_broadcast:
+            self.client.comm_params.timeout_connect = timeout  # noqa
         self.__response_check(resp)
 
+    @__write
+    def write_register(self, address: int, value: int) -> ModbusResponse:
+        """
+        :param address: Modbus register address
+        :param value: value to write
+        """
+        logging.debug(f"LedController: Writing register ({self.slave_id}): {address}={value}")
+        return self.client.write_register(address=address, slave=self.slave_id, value=value)
+
+    @__write
+    def write_registers(self, address: int, values: List[int]) -> ModbusResponse:
+        """
+        :param address: Modbus register address
+        :param values: values to write
+        """
+        logging.debug(f"LedController: Writing registers ({self.slave_id}): {address}={values}")
+        return self.client.write_registers(address=address, slave=self.slave_id, values=values)
+
     def set_red(self, value: int):
         self.write_register(REG.LED_R.value, value)
 
     def set_green(self, value: int):
         self.write_register(REG.LED_G.value, value)
 
     def set_blue(self, value: int):
         self.write_register(REG.LED_B.value, value)
 
     def set_white(self, value: int):
         self.write_register(REG.LED_W.value, value)
 
-    def set_rgb(self, red: int, green: int, blue: int, active: bool = True):
-        self.write_register(REG.LED_LIVE.value, 0)
-        self.write_register(REG.LED_R.value, red)
-        self.write_register(REG.LED_G.value, green)
-        self.write_register(REG.LED_B.value, blue)
-        if active:
-            self.write_register(REG.LED_LIVE.value, 1)
-
-    def set_rgbw(self, red: int, green: int, blue: int, white: int, active: bool = True):
-        self.write_register(REG.LED_LIVE.value, 0)
-        self.write_register(REG.LED_R.value, red)
-        self.write_register(REG.LED_G.value, green)
-        self.write_register(REG.LED_B.value, blue)
-        self.write_register(REG.LED_W.value, white)
-        if active:
-            self.write_register(REG.LED_LIVE.value, 1)
+    def set_rgb(self, red: int, green: int, blue: int):
+        self.write_registers(REG.LED_R.value, [red, green, blue])
+
+    def set_rgbw(self, red: int, green: int, blue: int, white: int):
+        self.write_registers(REG.LED_R.value, [red, green, blue, white])
+
+    def set_live_mode(self, value: bool):
+        self.write_register(REG.LED_LIVE.value, 1 if value else 0)
 
     def get_rgbw(self) -> List[int]:
         return self.read_register(REG.LED_R.value, count=4)
 
     def get_rgb(self) -> List[int]:
         return self.read_register(REG.LED_R.value, count=3)
 
     def get_red(self) -> int:
         return self.read_register(REG.LED_R.value)
 
+    def get_live_mode(self) -> int:
+        return self.read_register(REG.LED_LIVE.value)
+
     def get_green(self) -> int:
         return self.read_register(REG.LED_G.value)
 
     def get_blue(self) -> int:
         return self.read_register(REG.LED_B.value)
 
     def get_white(self) -> int:
@@ -153,33 +163,27 @@
     def set_serial_baudrate(self, value: int):
         self.write_register(REG.EE_SBAUD.value, value)
 
     def set_serial_parity(self, value: int):
         self.write_register(REG.EE_SPAR.value, value)
 
     def set_channel_configuration(self, red: int, green: int, blue: int, white: int):
-        self.write_register(REG.EE_LCH_R.value, red)
-        self.write_register(REG.EE_LCH_G.value, green)
-        self.write_register(REG.EE_LCH_B.value, blue)
-        self.write_register(REG.EE_LCH_W.value, white)
+        self.write_registers(REG.EE_LCH_R.value, [red, green, blue, white])
 
     def set_greeting_enable(self, value: bool):
         self.write_register(REG.EE_GR.value, value)
 
     def set_px_enable(self, value: bool):
         self.write_register(REG.EE_PXEN.value, value)
 
     def set_default_pwm_cycle(self, value: int):
         self.write_register(REG.EE_PWMC.value, value)
 
     def set_default_rgbw(self, red: int, green: int, blue: int, white: int):
-        self.write_register(REG.EE_LDF_R.value, red)
-        self.write_register(REG.EE_LDF_G.value, green)
-        self.write_register(REG.EE_LDF_B.value, blue)
-        self.write_register(REG.EE_LDF_W.value, white)
+        self.write_registers(REG.EE_LDF_R.value, [red, green, blue, white])
 
     def set_default_transition_time(self, value: int):
         self.write_register(REG.EE_LDF_TR.value, value)
 
     def get_mb_slave_id(self) -> int:
         return self.read_register(REG.EE_MBADDR.value)
```

### Comparing `ledsc-1.0.1/ledsc.egg-info/PKG-INFO` & `ledsc-1.0.2/ledsc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

