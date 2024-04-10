# Comparing `tmp/nicostick-0.0.3.tar.gz` & `tmp/nicostick-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicostick-0.0.3.tar", max compression
+gzip compressed data, was "nicostick-0.1.0.tar", max compression
```

## Comparing `nicostick-0.0.3.tar` & `nicostick-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2024-03-14 16:04:21.645640 nicostick-0.0.3/LICENSE
--rw-r--r--   0        0        0      186 2024-03-14 16:04:21.645640 nicostick-0.0.3/README.md
--rw-r--r--   0        0        0       49 2024-03-14 16:04:21.645640 nicostick-0.0.3/nicostick/__init__.py
--rw-r--r--   0        0        0       39 2024-03-14 16:04:21.645640 nicostick-0.0.3/nicostick/const.py
--rw-r--r--   0        0        0    11968 2024-03-14 16:04:21.645640 nicostick-0.0.3/nicostick/controller.py
--rw-r--r--   0        0        0      881 2024-03-14 16:04:21.645640 nicostick-0.0.3/nicostick/models.py
--rw-r--r--   0        0        0     7333 2024-03-14 16:04:21.645640 nicostick-0.0.3/nicostick/protocol.py
--rw-r--r--   0        0        0     1457 2024-03-14 16:04:21.645640 nicostick-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 nicostick-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-10 19:31:19.301595 nicostick-0.1.0/LICENSE
+-rw-r--r--   0        0        0      186 2024-04-10 19:31:19.301595 nicostick-0.1.0/README.md
+-rw-r--r--   0        0        0       49 2024-04-10 19:31:19.301595 nicostick-0.1.0/nicostick/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-10 19:31:19.301595 nicostick-0.1.0/nicostick/const.py
+-rw-r--r--   0        0        0    12680 2024-04-10 19:31:19.301595 nicostick-0.1.0/nicostick/controller.py
+-rw-r--r--   0        0        0      881 2024-04-10 19:31:19.301595 nicostick-0.1.0/nicostick/models.py
+-rw-r--r--   0        0        0     7616 2024-04-10 19:31:19.301595 nicostick-0.1.0/nicostick/protocol.py
+-rw-r--r--   0        0        0     1457 2024-04-10 19:31:19.301595 nicostick-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 nicostick-0.1.0/PKG-INFO
```

### Comparing `nicostick-0.0.3/LICENSE` & `nicostick-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nicostick-0.0.3/nicostick/controller.py` & `nicostick-0.1.0/nicostick/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,33 @@
     def __init__(self, address, udp_port=2430, tcp_port=2431, password=None):
         self._address = address
         self._udp_port = udp_port
         self._tcp_port = tcp_port
         self._password = password
         self._protocol = Stick3Protocol()
         self._state = Stick3State()
+        if self._password:
+            self._need_authentication = True
+        else:
+            self._need_authentication = False
 
     # I have not seen the Stick respond on UDP, so we will just fire and forget
     async def send_udp(self, data):
         _LOGGER.debug('Sending UDP: %s', data.hex())
         with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
             s.sendto(data, (self._address, self._udp_port))
             # data=s.recvfrom(1024)
             # print('Received UDP:', data.hex())
 
     async def open_tcp(self):
         self._reader, self._writer = await asyncio.open_connection(self._address, self._tcp_port)
         if self._password:
             self._need_authentication = True
+        else:
+            self._need_authentication = False
         # self.tcp_read_handler = asyncio.create_task(self.tcp_handler())
 
     async def send_tcp(self, data):
         if self._need_authentication:
             # turn off need_authentication so we don't get stuck in a loop
             # I guess there is possibility of a race condition here
             self._need_authentication = False
@@ -160,16 +166,16 @@
         _LOGGER.debug('Auth result: %d', auth_result_code)
         self._auth_result_code = auth_result_code
         if hasattr(self, '_auth_future') and self._auth_future:
             fut = self._auth_future
             self._auth_future = None
             fut.set_result(auth_result_code)
 
-    async def start_scene(self, scene_nr, zone_sync_id, dimmer_val, speed_val, color_val):
-        data = self._protocol.scene_trigger_encode(scene_nr, zone_sync_id, 1, dimmer_val, speed_val, color_val)
+    async def start_scene(self, scene_nr, zone_sync_id, dimmer_val, speed_val, color_val, cmd=0x01):
+        data = self._protocol.scene_trigger_encode(scene_nr, zone_sync_id, cmd, dimmer_val, speed_val, color_val)
         # await self.send_udp(data)
         await self.send_tcp(data)
 
     async def read_file(self, file_name):
         if hasattr(self, 'file_name') and self.file_name:
             raise ValueError('File name already set.')
         self.file_name = file_name
@@ -280,14 +286,23 @@
             _LOGGER.debug(f"Starting scene {scene_index}:{scene_name} on zone {zone_id}")
             await self.start_scene(scene_index, zone_id, 0, 0, 0)
         except ValueError:
             _LOGGER.warning(f"Scene {scene_name} not found")
         except KeyError:
             _LOGGER.warning(f"Zone {zone_id} not found")
 
+    async def set_brightness(self, zone_id, brightness):
+        # we need the current to be able to set brightness
+        scene_index = self._state.zone_states[zone_id].running_scene
+        await self.start_scene(scene_index, zone_id, int(brightness), 0, 0,cmd=0x05)
+
+    async def set_rgb_color(self, zone_id, r, g, b):
+        scene_index = self._state.zone_states[zone_id].running_scene
+        await self.start_scene(scene_index, zone_id, 0, 0, (r << 16) + (g << 8) + b,cmd=0x07)
+
     async def read_show_map_file(self):
         file_data = await self.read_file('Show1/show_map.xml')
         root = ET.fromstring(file_data)
         # We don't know how to work the channels so skip that for now
         # Scenes
         scenes = {}
         for item in root.findall('Scenes/item'):
@@ -300,7 +315,8 @@
 
         self._state.scenes = scenes
         self._state.zones = zones
 
     async def update(self):
         for zone_id in self._state.zones.keys():
             await self.send_query_zone_status(zone_id)
+        return True
```

### Comparing `nicostick-0.0.3/nicostick/models.py` & `nicostick-0.1.0/nicostick/models.py`

 * *Files identical despite different names*

### Comparing `nicostick-0.0.3/nicostick/protocol.py` & `nicostick-0.1.0/nicostick/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def tcp_get_salt_encode(self, stamp):
         return struct.pack('<8sHQ6x', ID, OpCodes.OpTcpGetSalt.value, stamp)
 
     def tcp_authenticate_encode(self, stamp, login, salt, signature):
         return struct.pack('<8sHQ32s32s32s6x', ID, OpCodes.OpTcpAuthentificate.value, stamp, login, salt, signature)
 
     def auth_message_encode(self, ID, opcode, stamp, login, salt):
-        print(ID, opcode, stamp, login, salt)
+        #print(ID, opcode, stamp, login, salt)
         return struct.pack('<8sHQ32s32s', ID, opcode, stamp, login, salt)
 
     def decode(self, data):
         _LOGGER.debug('Decoding: %s', data.hex())
         (id, code) = struct.unpack('<8sH', data[:10])
         opcode = OpCodes(code)
         if opcode == OpCodes.OpFileData:
@@ -104,14 +104,15 @@
         # print(f"Packet: {packet.hex()
         # (file_name,file_end,data_size,file_data) = struct.unpack(f'<32sBxh2x{rest}p',data)
         (file_name, file_end, data_size) = struct.unpack('<32sBxh2x', data[:38])
         file_data = data[38:]
         return [file_name, file_end, data_size, file_data]
 
     def decode_zone_status(self, data):
+        _LOGGER.debug('Decoding zone status reply: %s', data.hex())
         (
             stamp,
             zone_id,
             running_scene,
             scene_state,
             dimmer,
             speed,
@@ -124,15 +125,20 @@
         running_scene = None if running_scene == 0xFFFF else running_scene
         dimmer = None if dimmer == 0xFFFF else dimmer
         speed = None if speed == 0xFFFF else speed
         # docs says ColorRGB:0x00BBGGRR; 0xFFFFFFFF when not applied
         # but I only get =0x0FFFFFFF for N/A
         color_rgb = None if color_rgb == 0x0FFFFFFF else color_rgb
         if color_rgb is not None:
-            color_rgb = color_rgb & 0xFF, (color_rgb >> 8) & 0xFF, (color_rgb >> 16) & 0xFF
+            _LOGGER.debug('Decoding color: %x', color_rgb)
+
+            #color_rgb = color_rgb & 0xFF , (color_rgb >> 8) & 0xFF,(color_rgb >> 16) & 0xFF
+            color_rgb = (color_rgb >> 16) & 0xFF,  (color_rgb >> 8) & 0xFF,color_rgb & 0xFF ,
+            _LOGGER.debug('Decoded color: %s', color_rgb)
+
         color_sat = None if color_sat == 0xFFFF else color_sat  # docs says always 0xFFFF
         extra_color1 = None if extra_color1 == 0xFFFF else extra_color1
         extra_color2 = None if extra_color2 == 0xFFFF else extra_color2
         extra_color3 = None if extra_color3 == 0xFFFF else extra_color3
 
         return [
             stamp,
```

### Comparing `nicostick-0.0.3/pyproject.toml` & `nicostick-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nicostick"
-version = "0.0.3"
+version = "0.1.0"
 description = "Python package for interfacing with the Nicolaudie Stick3-DE DMX controller over Ethernet"
 authors = ["Yngvi Thor Sigurjonsson <blitzkopf@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/blitzkopf/shadeorb"
 repository = "https://github.com/blitzkopf/shadeorb"
 keywords = ["nicolaudie", "stick3", "dmx", "lighting", "controller"]
```

### Comparing `nicostick-0.0.3/PKG-INFO` & `nicostick-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicostick
-Version: 0.0.3
+Version: 0.1.0
 Summary: Python package for interfacing with the Nicolaudie Stick3-DE DMX controller over Ethernet
 Home-page: https://github.com/blitzkopf/shadeorb
 License: MIT
 Keywords: nicolaudie,stick3,dmx,lighting,controller
 Author: Yngvi Thor Sigurjonsson
 Author-email: blitzkopf@gmail.com
 Requires-Python: >=3.10,<3.13
```

