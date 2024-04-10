# Comparing `tmp/thonny-etboard-micropython-firmware-v2-1.0.4.tar.gz` & `tmp/thonny-etboard-micropython-firmware-v2-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-etboard-micropython-firmware-v2-1.0.4.tar", last modified: Wed Apr 10 11:43:44 2024, max compression
+gzip compressed data, was "thonny-etboard-micropython-firmware-v2-1.0.5.tar", last modified: Wed Apr 10 11:49:21 2024, max compression
```

## Comparing `thonny-etboard-micropython-firmware-v2-1.0.4.tar` & `thonny-etboard-micropython-firmware-v2-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 11:43:44.174289 thonny-etboard-micropython-firmware-v2-1.0.4/
--rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-v2-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      637 2024-04-10 11:43:44.174289 thonny-etboard-micropython-firmware-v2-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       90 2024-04-10 09:18:03.000000 thonny-etboard-micropython-firmware-v2-1.0.4/README.md
--rw-rw-rw-   0        0        0      108 2024-04-10 09:21:20.000000 thonny-etboard-micropython-firmware-v2-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 11:43:44.175286 thonny-etboard-micropython-firmware-v2-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      956 2024-04-10 11:43:34.000000 thonny-etboard-micropython-firmware-v2-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:43:44.167806 thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/
--rw-rw-rw-   0        0        0      637 2024-04-10 11:43:44.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-10 11:43:44.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 11:43:44.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 11:43:44.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 11:43:44.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 11:43:44.159532 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:43:44.169799 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/
--rw-rw-rw-   0        0        0     1106 2024-04-10 07:05:59.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:43:44.160531 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/etboard/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:43:44.172295 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/
--rw-rw-rw-   0        0        0  1488656 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
--rw-rw-rw-   0        0        0  1556784 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
--rw-rw-rw-   0        0        0     3507 2024-04-10 06:54:37.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py
--rw-rw-rw-   0        0        0     5144 2024-04-10 07:21:45.000000 thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:49:21.890222 thonny-etboard-micropython-firmware-v2-1.0.5/
+-rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-v2-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      637 2024-04-10 11:49:21.890222 thonny-etboard-micropython-firmware-v2-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       90 2024-04-10 09:18:03.000000 thonny-etboard-micropython-firmware-v2-1.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-10 09:21:20.000000 thonny-etboard-micropython-firmware-v2-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 11:49:21.891219 thonny-etboard-micropython-firmware-v2-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      956 2024-04-10 11:48:29.000000 thonny-etboard-micropython-firmware-v2-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:49:21.883245 thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/
+-rw-rw-rw-   0        0        0      637 2024-04-10 11:49:21.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-04-10 11:49:21.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:49:21.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 11:49:21.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 11:49:21.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 11:49:21.869172 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:49:21.885239 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/
+-rw-rw-rw-   0        0        0     1106 2024-04-10 07:05:59.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:49:21.870168 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/etboard/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:49:21.888229 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/
+-rw-rw-rw-   0        0        0  1488656 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
+-rw-rw-rw-   0        0        0  1556784 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
+-rw-rw-rw-   0        0        0     3507 2024-04-10 06:54:37.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py
+-rw-rw-rw-   0        0        0     5144 2024-04-10 07:21:45.000000 thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/LICENSE` & `thonny-etboard-micropython-firmware-v2-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/PKG-INFO` & `thonny-etboard-micropython-firmware-v2-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-etboard-micropython-firmware-v2
-Version: 1.0.4
+Version: 1.0.5
 Summary: 이티보드 마이크로파이썬 펌웨어
 Home-page: http://et.ketri.re.kr/
 Author: KETRi
 Author-email: ketri3000@gmail.com
 Project-URL: Bug Tracker, http://et.ketri.re.kr/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/setup.py` & `thonny-etboard-micropython-firmware-v2-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thonny-etboard-micropython-firmware-v2",
-    version="1.0.4",
+    version="1.0.5",
     author="KETRi",
     author_email="ketri3000@gmail.com",
     description="이티보드 마이크로파이썬 펌웨어",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://et.ketri.re.kr/",
     project_urls={
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO` & `thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny-etboard-micropython-firmware-v2
-Version: 1.0.4
+Version: 1.0.5
 Summary: 이티보드 마이크로파이썬 펌웨어
 Home-page: http://et.ketri.re.kr/
 Author: KETRi
 Author-email: ketri3000@gmail.com
 Project-URL: Bug Tracker, http://et.ketri.re.kr/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt` & `thonny-etboard-micropython-firmware-v2-1.0.5/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/__init__.py` & `thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin` & `thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin` & `thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py` & `thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.4/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py` & `thonny-etboard-micropython-firmware-v2-1.0.5/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py`

 * *Files identical despite different names*

