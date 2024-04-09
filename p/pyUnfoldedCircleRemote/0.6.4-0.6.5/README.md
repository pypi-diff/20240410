# Comparing `tmp/pyunfoldedcircleremote-0.6.4.tar.gz` & `tmp/pyunfoldedcircleremote-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunfoldedcircleremote-0.6.4.tar", max compression
+gzip compressed data, was "pyunfoldedcircleremote-0.6.5.tar", max compression
```

## Comparing `pyunfoldedcircleremote-0.6.4.tar` & `pyunfoldedcircleremote-0.6.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.6.4/LICENSE
--rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.6.4/README.md
--rw-r--r--   0        0        0      604 2024-03-18 00:46:48.384086 pyunfoldedcircleremote-0.6.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.6.4/src/pyUnfoldedCircleRemote/__init__.py
--rw-r--r--   0        0        0      766 2024-03-18 00:46:24.936844 pyunfoldedcircleremote-0.6.4/src/pyUnfoldedCircleRemote/const.py
--rw-r--r--   0        0        0    63460 2024-03-18 00:46:34.997096 pyunfoldedcircleremote-0.6.4/src/pyUnfoldedCircleRemote/remote.py
--rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.6.4/src/pyUnfoldedCircleRemote/remote_websocket.py
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.6.5/LICENSE
+-rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.6.5/README.md
+-rw-r--r--   0        0        0      604 2024-04-09 22:59:05.713271 pyunfoldedcircleremote-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.6.5/src/pyUnfoldedCircleRemote/__init__.py
+-rw-r--r--   0        0        0      766 2024-03-18 00:46:24.936844 pyunfoldedcircleremote-0.6.5/src/pyUnfoldedCircleRemote/const.py
+-rw-r--r--   0        0        0    63499 2024-04-09 22:54:49.567411 pyunfoldedcircleremote-0.6.5/src/pyUnfoldedCircleRemote/remote.py
+-rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.6.5/src/pyUnfoldedCircleRemote/remote_websocket.py
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.6.5/PKG-INFO
```

### Comparing `pyunfoldedcircleremote-0.6.4/LICENSE` & `pyunfoldedcircleremote-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.6.4/pyproject.toml` & `pyunfoldedcircleremote-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUnfoldedCircleRemote"
-version = "0.6.4"
+version = "0.6.5"
 description = "A python library to interact with the Unfolded Circle Remote"
 authors = ["Jack Powell <jackjpowell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jackjpowell/py-unfolded-circle"
 packages = [{include = "pyUnfoldedCircleRemote", from = "src"}]
```

### Comparing `pyunfoldedcircleremote-0.6.4/src/pyUnfoldedCircleRemote/const.py` & `pyunfoldedcircleremote-0.6.5/src/pyUnfoldedCircleRemote/const.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.6.4/src/pyUnfoldedCircleRemote/remote.py` & `pyunfoldedcircleremote-0.6.5/src/pyUnfoldedCircleRemote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,15 +794,15 @@
         async with (
             self.client() as session,
             session.get(self.url("system/update")) as response,
         ):
             await self.raise_on_error(response)
             information = await response.json()
             self._update_in_progress = information["update_in_progress"]
-            self._next_update_check_date = information["next_check_date"]
+            # self._next_update_check_date = information["next_check_date"]
             self._sw_version = information["installed_version"]
             self._automatic_updates = information["update_check_enabled"]
             if "available" in information:
                 self._available_update = information["available"]
                 for update in self._available_update:
                     if update.get("channel") in ["STABLE", "TESTING"]:
                         if (
@@ -822,15 +822,15 @@
         async with (
             self.client() as session,
             session.put(self.url("system/update")) as response,
         ):
             await self.raise_on_error(response)
             information = await response.json()
             self._update_in_progress = information["update_in_progress"]
-            self._next_update_check_date = information["next_check_date"]
+            # self._next_update_check_date = information["next_check_date"]
             self._sw_version = information["installed_version"]
             self._automatic_updates = information["update_check_enabled"]
             if "available" in information:
                 self._available_update = information["available"]
             return information
 
     async def update_remote(self) -> str:
@@ -923,14 +923,16 @@
                 }
                 self._ir_custom.append(ir_data.copy())
             return self._ir_custom
 
     async def get_remote_codesets(self) -> list:
         """Get list of remote codesets."""
         ir_data = {}
+        if not self._remotes:
+            await self.get_remotes()
         for remote in self._remotes:
             async with (
                 self.client() as session,
                 session.get(
                     self.url("remotes/" + remote.get("entity_id") + "/ir")
                 ) as response,
             ):
@@ -1202,15 +1204,14 @@
             self.get_stats(),
             self.get_remote_display_settings(),
             self.get_remote_button_settings(),
             self.get_remote_sound_settings(),
             self.get_remote_haptic_settings(),
             self.get_remote_power_saving_settings(),
             self.get_activities(),
-            self.get_remotes(),
             self.get_remote_codesets(),
             self.get_docks(),
         )
         await group
 
         await self.get_activity_groups()
```

### Comparing `pyunfoldedcircleremote-0.6.4/src/pyUnfoldedCircleRemote/remote_websocket.py` & `pyunfoldedcircleremote-0.6.5/src/pyUnfoldedCircleRemote/remote_websocket.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.6.4/PKG-INFO` & `pyunfoldedcircleremote-0.6.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUnfoldedCircleRemote
-Version: 0.6.4
+Version: 0.6.5
 Summary: A python library to interact with the Unfolded Circle Remote
 Home-page: https://github.com/jackjpowell/py-unfolded-circle
 License: MIT
 Author: Jack Powell
 Author-email: jackjpowell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

