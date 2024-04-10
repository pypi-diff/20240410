# Comparing `tmp/adb_connector_python-1.1.6-py3-none-any.whl.zip` & `tmp/adb_connector_python-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11471 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    38713 b- defN 24-Apr-10 09:42 adb_connector_python/connector.py
--rwxrwxrwx  2.0 unx     1088 b- defN 24-Apr-10 09:44 adb_connector_python-1.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5452 b- defN 24-Apr-10 09:44 adb_connector_python-1.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 09:44 adb_connector_python-1.1.6.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       21 b- defN 24-Apr-10 09:44 adb_connector_python-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      542 b- defN 24-Apr-10 09:44 adb_connector_python-1.1.6.dist-info/RECORD
-6 files, 45908 bytes uncompressed, 10479 bytes compressed:  77.2%
+Zip file size: 11484 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    38896 b- defN 24-Apr-10 12:56 adb_connector_python/connector.py
+-rwxrwxrwx  2.0 unx     1088 b- defN 24-Apr-10 12:56 adb_connector_python-1.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5452 b- defN 24-Apr-10 12:56 adb_connector_python-1.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 12:56 adb_connector_python-1.1.7.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       21 b- defN 24-Apr-10 12:56 adb_connector_python-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      542 b- defN 24-Apr-10 12:56 adb_connector_python-1.1.7.dist-info/RECORD
+6 files, 46091 bytes uncompressed, 10492 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: adb_connector_python/connector.py
 Comment: 
 
-Filename: adb_connector_python-1.1.6.dist-info/LICENSE
+Filename: adb_connector_python-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: adb_connector_python-1.1.6.dist-info/METADATA
+Filename: adb_connector_python-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: adb_connector_python-1.1.6.dist-info/WHEEL
+Filename: adb_connector_python-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: adb_connector_python-1.1.6.dist-info/top_level.txt
+Filename: adb_connector_python-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: adb_connector_python-1.1.6.dist-info/RECORD
+Filename: adb_connector_python-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adb_connector_python/connector.py

```diff
@@ -68,14 +68,15 @@
 
 # adb command
 CMD_START_ADB: str = "adb start-server"
 CMD_KILL_ADB: str = "adb kill-server"
 CMD_LIST_DEVICES: str = "adb devices"
 
 
+
 def IS_ADB_RUNNING_CMD() -> str:
     match platform:
         case "win32":
             return "tasklist | findstr adb"
         case "linux" | "darwin":
             return "ps aux | grep adb"
         case _:
@@ -147,17 +148,14 @@
     * voice_assistant : toggle voice assistant, like saying 'ok google'
     * volume_up / volume_down : to raise or low the volume, provide 'times' to define how many times repeat the action
     * brightness_up / brightness_down : to raise or low brightness, provide 'times' to define how many times repeat the action
     """
 
     def __init__(self) -> None:
         # if adb shell is not running, raise a RuntimeError exception
-
-
-
         if not self.is_adb_running():
             raise RuntimeError(
                 "ADB is not running, please start it with 'adb start-server'")
 
         self.ADB_DATA = execute("adb --version")
         self.ADB_VERSION = self.ADB_DATA.split()[4]
         self.ADB_EXECUTABLE = self.ADB_DATA.split()[9]
@@ -613,30 +611,35 @@
                     device_id: str = self.get_first_avaiable_device()["id"]
                 return execute_keyevent(COMMAND_SWIPE.format(
                     device_id, from_x, from_y, to_x, to_y))
             else:
                 print(colored(" > ERROR : phone need to be awake","red"))
                 return False
             
-    def multitap(self, x: int, y: int,times:int= 2,milliseconds:int=0, device_id: str = None) -> bool:
+    def multitap(self, x: int, y: int,times:int,milliseconds:int=0, device_id: str = None) -> bool:
         """
 You can use this function to tap on the screen giving x and y at very fast time providing milliseconds
 between a tap and an other and times to express how many times will be tapped
         """
         if not self.get_first_avaiable_device():
             raise RuntimeError("no device detected")
         else:
             self._basic_device_check()
             if not device_id:
                 if len(self.list_devices()) == 0: raise RuntimeError("a device must be connected")
                 device_id = self.get_first_avaiable_device()["id"]
+        if times > 0:
+            for _ in range(times):
+                execute_keyevent(COMMAND_TAP.format(device_id, x, y))
+                sleep(milliseconds / 1000)
+        else:
+            while True:
+                execute_keyevent(COMMAND_TAP.format(device_id, x, y))
+                sleep(milliseconds / 1000)
 
-        for _ in range(times):
-            execute_keyevent(COMMAND_TAP.format(device_id, x, y))
-            sleep(milliseconds / 1000)
           
 
 
     def precision_tap(self,instructions:list, device_id: str = None)->None:
         if not self.get_first_avaiable_device():
             raise RuntimeError("no device detected")
         else:
```

## Comparing `adb_connector_python-1.1.6.dist-info/LICENSE` & `adb_connector_python-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `adb_connector_python-1.1.6.dist-info/METADATA` & `adb_connector_python-1.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-connector-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: A simple python package to interface with adb
 Author: Giuseppe Gravante
 License: MIT License
         
         Copyright (c) 2023 Giuseppe7887
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `adb_connector_python-1.1.6.dist-info/RECORD` & `adb_connector_python-1.1.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-adb_connector_python/connector.py,sha256=AzNlR8x4F8ddDA__8n-4hSfkwY2s1RTU7eAR1h_rmww,38713
-adb_connector_python-1.1.6.dist-info/LICENSE,sha256=I_ByMPSnNu3xgizHvEHpoes3YsmO8uQx80UpXk2oWGc,1088
-adb_connector_python-1.1.6.dist-info/METADATA,sha256=-2-rMqOUg8S8cumuqs7jVMmBvl2NfJHSQ_Kq-cdcfUg,5452
-adb_connector_python-1.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-adb_connector_python-1.1.6.dist-info/top_level.txt,sha256=Lm728SyX737VLY8s8V37rYl62-Gs84c1b7py5lKl8Xc,21
-adb_connector_python-1.1.6.dist-info/RECORD,,
+adb_connector_python/connector.py,sha256=2rUbe3hT1FnzR16PM5FXcHAbL3jZMoKeieu1132KOhE,38896
+adb_connector_python-1.1.7.dist-info/LICENSE,sha256=I_ByMPSnNu3xgizHvEHpoes3YsmO8uQx80UpXk2oWGc,1088
+adb_connector_python-1.1.7.dist-info/METADATA,sha256=cSHy_7tw2vWmwFjqteyGv8Fq6MaKMcY4XYY4NPJdwww,5452
+adb_connector_python-1.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+adb_connector_python-1.1.7.dist-info/top_level.txt,sha256=Lm728SyX737VLY8s8V37rYl62-Gs84c1b7py5lKl8Xc,21
+adb_connector_python-1.1.7.dist-info/RECORD,,
```

