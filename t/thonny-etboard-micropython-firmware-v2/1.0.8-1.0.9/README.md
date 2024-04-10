# Comparing `tmp/thonny-etboard-micropython-firmware-v2-1.0.8.tar.gz` & `tmp/thonny-etboard-micropython-firmware-v2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-etboard-micropython-firmware-v2-1.0.8.tar", last modified: Wed Apr 10 12:16:09 2024, max compression
+gzip compressed data, was "thonny-etboard-micropython-firmware-v2-1.0.9.tar", last modified: Wed Apr 10 12:30:39 2024, max compression
```

## Comparing `thonny-etboard-micropython-firmware-v2-1.0.8.tar` & `thonny-etboard-micropython-firmware-v2-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:16:09.657038 thonny-etboard-micropython-firmware-v2-1.0.8/
--rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-v2-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      656 2024-04-10 12:16:09.657038 thonny-etboard-micropython-firmware-v2-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       95 2024-04-10 12:15:53.000000 thonny-etboard-micropython-firmware-v2-1.0.8/README.md
--rw-rw-rw-   0        0        0      108 2024-04-10 09:21:20.000000 thonny-etboard-micropython-firmware-v2-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 12:16:09.659031 thonny-etboard-micropython-firmware-v2-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      976 2024-04-10 12:16:03.000000 thonny-etboard-micropython-firmware-v2-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:16:09.650318 thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/
--rw-rw-rw-   0        0        0      656 2024-04-10 12:16:09.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-10 12:16:09.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:16:09.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 12:16:09.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 12:16:09.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 12:16:09.634991 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/
-drwxrwxrwx   0        0        0        0 2024-04-10 12:16:09.651314 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/
--rw-rw-rw-   0        0        0     1106 2024-04-10 07:05:59.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:16:09.634991 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/etboard/
-drwxrwxrwx   0        0        0        0 2024-04-10 12:16:09.654047 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/
--rw-rw-rw-   0        0        0  1488656 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
--rw-rw-rw-   0        0        0  1556784 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
--rw-rw-rw-   0        0        0     3507 2024-04-10 06:54:37.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py
--rw-rw-rw-   0        0        0     5144 2024-04-10 07:21:45.000000 thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:30:39.830816 thonny-etboard-micropython-firmware-v2-1.0.9/
+-rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-v2-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      657 2024-04-10 12:30:39.830816 thonny-etboard-micropython-firmware-v2-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2024-04-10 12:15:53.000000 thonny-etboard-micropython-firmware-v2-1.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-10 09:21:20.000000 thonny-etboard-micropython-firmware-v2-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:30:39.831813 thonny-etboard-micropython-firmware-v2-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      977 2024-04-10 12:24:46.000000 thonny-etboard-micropython-firmware-v2-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:30:39.824280 thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/
+-rw-rw-rw-   0        0        0      657 2024-04-10 12:30:39.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2024-04-10 12:30:39.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:30:39.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 12:30:39.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 12:30:39.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 12:30:39.815643 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/
+drwxrwxrwx   0        0        0        0 2024-04-10 12:30:39.825278 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/
+-rw-rw-rw-   0        0        0     1106 2024-04-10 07:05:59.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:30:39.815643 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/etboard/
+drwxrwxrwx   0        0        0        0 2024-04-10 12:30:39.828822 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/
+-rw-rw-rw-   0        0        0      233 2024-04-10 12:29:43.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/ReadMe.md
+-rw-rw-rw-   0        0        0  1488656 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
+-rw-rw-rw-   0        0        0  1556784 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
+-rw-rw-rw-   0        0        0     3507 2024-04-10 06:54:37.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py
+-rw-rw-rw-   0        0        0     5144 2024-04-10 07:21:45.000000 thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/LICENSE` & `thonny-etboard-micropython-firmware-v2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/PKG-INFO` & `thonny-etboard-micropython-firmware-v2-1.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: thonny-etboard-micropython-firmware-v2
-Version: 1.0.8
+Version: 1.0.9
 Summary: 이티보드 마이크로파이썬 펌웨어
 Home-page: http://et.ketri.re.kr/
 Author: KETRi
 Author-email: ketri3000@gmail.com
 License: MIT
 Project-URL: Bug Tracker, http://et.ketri.re.kr/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: thonny>=3.3.11
 
 Thonny 이티보드 펌웨어와 인터프리터 설정을 포함하는 플러그인 입니다.
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/setup.py` & `thonny-etboard-micropython-firmware-v2-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thonny-etboard-micropython-firmware-v2",
-    version="1.0.8",
+    version="1.0.9",
     author="KETRi",
     author_email="ketri3000@gmail.com",
     description="이티보드 마이크로파이썬 펌웨어",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://et.ketri.re.kr/",
     project_urls={
@@ -19,10 +19,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=["thonnycontrib.thonny_etboard_firmware_v2"],
     package_data={"thonnycontrib.thonny_etboard_firmware_v2" : ["*", "*/*", "*/*/*", "*/*/*/*", "*/*/*/*/*"]},
     install_requires = ["thonny>=3.3.11"],
-    python_requires=">=3.6",
+    python_requires=">=3.10",
     license='MIT',
 )
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO` & `thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: thonny-etboard-micropython-firmware-v2
-Version: 1.0.8
+Version: 1.0.9
 Summary: 이티보드 마이크로파이썬 펌웨어
 Home-page: http://et.ketri.re.kr/
 Author: KETRi
 Author-email: ketri3000@gmail.com
 License: MIT
 Project-URL: Bug Tracker, http://et.ketri.re.kr/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: thonny>=3.3.11
 
 Thonny 이티보드 펌웨어와 인터프리터 설정을 포함하는 플러그인 입니다.
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt` & `thonny-etboard-micropython-firmware-v2-1.0.9/thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 thonny_etboard_micropython_firmware_v2.egg-info/SOURCES.txt
 thonny_etboard_micropython_firmware_v2.egg-info/dependency_links.txt
 thonny_etboard_micropython_firmware_v2.egg-info/requires.txt
 thonny_etboard_micropython_firmware_v2.egg-info/top_level.txt
 thonnycontrib/thonny_etboard_firmware_v2/__init__.py
 thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py
 thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py
+thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/ReadMe.md
 thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
 thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
```

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/__init__.py` & `thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin` & `thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin` & `thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py` & `thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/thonny_v3.py`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-v2-1.0.8/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py` & `thonny-etboard-micropython-firmware-v2-1.0.9/thonnycontrib/thonny_etboard_firmware_v2/thonny_v4.py`

 * *Files identical despite different names*

