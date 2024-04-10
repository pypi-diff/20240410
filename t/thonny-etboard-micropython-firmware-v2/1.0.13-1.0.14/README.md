# Comparing `tmp/thonny-etboard-micropython-firmware-v2-1.0.13.tar.gz` & `tmp/thonny-etboard-micropython-firmware-v2-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-etboard-micropython-firmware-v2-1.0.13.tar", last modified: Wed Apr 10 13:42:37 2024, max compression
+gzip compressed data, was "thonny-etboard-micropython-firmware-v2-1.0.14.tar", last modified: Wed Apr 10 13:52:34 2024, max compression
```

## Comparing `thonny-etboard-micropython-firmware-v2-1.0.13.tar` & `thonny-etboard-micropython-firmware-v2-1.0.14.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 13:42:37.834880 thonny-etboard-micropython-firmware-v2-1.0.13/
--rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-v2-1.0.13/LICENSE
--rw-rw-rw-   0        0        0      676 2024-04-10 13:42:37.834880 thonny-etboard-micropython-firmware-v2-1.0.13/PKG-INFO
--rw-rw-rw-   0        0        0       95 2024-04-10 12:15:53.000000 thonny-etboard-micropython-firmware-v2-1.0.13/README.md
--rw-rw-rw-   0        0        0      108 2024-04-10 09:21:20.000000 thonny-etboard-micropython-firmware-v2-1.0.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 13:42:37.835879 thonny-etboard-micropython-firmware-v2-1.0.13/setup.cfg
--rw-rw-rw-   0        0        0      996 2024-04-10 13:42:22.000000 thonny-etboard-micropython-firmware-v2-1.0.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:42:37.826042 thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/
--rw-rw-rw-   0        0        0      676 2024-04-10 13:42:37.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2024-04-10 13:42:37.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:42:37.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 13:42:37.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 13:42:37.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 13:42:37.804614 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/
-drwxrwxrwx   0        0        0        0 2024-04-10 13:42:37.829032 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/
--rw-rw-rw-   0        0        0     1106 2024-04-10 07:05:59.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:42:37.805610 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/etboard/
-drwxrwxrwx   0        0        0        0 2024-04-10 13:42:37.833019 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/
--rw-rw-rw-   0        0        0      233 2024-04-10 12:29:43.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/ReadMe.md
--rw-rw-rw-   0        0        0  1488656 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
--rw-rw-rw-   0        0        0  1556784 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
--rw-rw-rw-   0        0        0     4218 2024-04-10 12:47:19.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py
--rw-rw-rw-   0        0        0     5144 2024-04-10 07:21:45.000000 thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:52:34.272946 thonny-etboard-micropython-firmware-v2-1.0.14/
+-rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-v2-1.0.14/LICENSE
+-rw-rw-rw-   0        0        0      676 2024-04-10 13:52:34.271950 thonny-etboard-micropython-firmware-v2-1.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2024-04-10 12:15:53.000000 thonny-etboard-micropython-firmware-v2-1.0.14/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-10 09:21:20.000000 thonny-etboard-micropython-firmware-v2-1.0.14/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 13:52:34.273943 thonny-etboard-micropython-firmware-v2-1.0.14/setup.cfg
+-rw-rw-rw-   0        0        0      996 2024-04-10 13:52:01.000000 thonny-etboard-micropython-firmware-v2-1.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:52:34.264973 thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/
+-rw-rw-rw-   0        0        0      676 2024-04-10 13:52:34.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2024-04-10 13:52:34.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 13:52:34.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 13:52:34.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 13:52:34.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 13:52:34.250648 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/
+drwxrwxrwx   0        0        0        0 2024-04-10 13:52:34.266966 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/
+-rw-rw-rw-   0        0        0     1106 2024-04-10 07:05:59.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:52:34.250648 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/etboard/
+drwxrwxrwx   0        0        0        0 2024-04-10 13:52:34.269956 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/
+-rw-rw-rw-   0        0        0      233 2024-04-10 12:29:43.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/ReadMe.md
+-rw-rw-rw-   0        0        0  1488656 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
+-rw-rw-rw-   0        0        0  1556784 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
+-rw-rw-rw-   0        0        0     4218 2024-04-10 12:47:19.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py
+-rw-rw-rw-   0        0        0     5172 2024-04-10 13:48:02.000000 thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/LICENSE` & `thonny-etboard-micropython-firmware-v2-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/PKG-INFO` & `thonny-etboard-micropython-firmware-v2-1.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-etboard-micropython-firmware-v2
-Version: 1.0.13
+Version: 1.0.14
 Summary: 이티보드 마이크로파이썬 펌웨어 - Thonny V4 이상
 Home-page: http://et.ketri.re.kr/
 Author: KETRi
 Author-email: ketri3000@gmail.com
 License: MIT
 Project-URL: Bug Tracker, http://et.ketri.re.kr/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/setup.py` & `thonny-etboard-micropython-firmware-v2-1.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thonny-etboard-micropython-firmware-v2",
-    version="1.0.13",
+    version="1.0.14",
     author="KETRi",
     author_email="ketri3000@gmail.com",
     description="이티보드 마이크로파이썬 펌웨어 - Thonny V4 이상",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://et.ketri.re.kr/",
     project_urls={
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO` & `thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-etboard-micropython-firmware-v2
-Version: 1.0.13
+Version: 1.0.14
 Summary: 이티보드 마이크로파이썬 펌웨어 - Thonny V4 이상
 Home-page: http://et.ketri.re.kr/
 Author: KETRi
 Author-email: ketri3000@gmail.com
 License: MIT
 Project-URL: Bug Tracker, http://et.ketri.re.kr/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt` & `thonny-etboard-micropython-firmware-v2-1.0.14/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/__init__.py` & `thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin` & `thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin` & `thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py` & `thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.13/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py` & `thonny-etboard-micropython-firmware-v2-1.0.14/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # import for custom dialog
 from thonny.plugins.micropython.esptool_dialog import ESPFlashingDialog
 # ==========================================================================================
 class ETboardESPFlashingDialog(ESPFlashingDialog):
 # ==========================================================================================
     def get_variants_url(self) -> str:
         #return f"https://raw.githubusercontent.com/thonny/thonny/master/data/{self.firmware_name.lower()}-variants-esptool.json"
-        return f"https://raw.githubusercontent.com/etboard/thonny/master/data/{self.firmware_name.lower()}-variants-esptool.json"
+        return f"https://raw.githubusercontent.com/etboard/ETboard_Public_Data/master/3dparty/thonny/data/{self.firmware_name.lower()}-variants-esptool.json"
 
 # ==========================================================================================        
 class ETBoardMenu:
 # ==========================================================================================    
     def __init__(self):
         self.workbench = get_workbench()
```

