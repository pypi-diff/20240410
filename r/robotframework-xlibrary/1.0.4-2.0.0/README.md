# Comparing `tmp/robotframework-xlibrary-1.0.4.tar.gz` & `tmp/robotframework-xlibrary-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-1.0.4.tar", last modified: Tue Apr  9 09:55:36 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-2.0.0.tar", last modified: Wed Apr 10 02:48:17 2024, max compression
```

## Comparing `robotframework-xlibrary-1.0.4.tar` & `robotframework-xlibrary-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1584 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-09 09:54:07.000000 robotframework-xlibrary-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/XLibrary/
--rw-rw-rw-   0        0        0     1792 2024-04-09 09:39:59.000000 robotframework-xlibrary-1.0.4/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-1.0.4/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 09:53:52.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     1584 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1584 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-04-10 02:47:01.000000 robotframework-xlibrary-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/XLibrary/
+-rw-rw-rw-   0        0        0     1792 2024-04-09 09:39:59.000000 robotframework-xlibrary-2.0.0/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-2.0.0/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     3136 2024-04-10 02:46:51.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     1584 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-1.0.4/PKG-INFO` & `robotframework-xlibrary-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 1.0.4
+Version: 2.0.0
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-1.0.4/README.md` & `robotframework-xlibrary-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-1.0.4/setup.py` & `robotframework-xlibrary-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="1.0.4",
+    version="2.0.0",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Test Library for robotframework-xlibrary",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-1.0.4/src/XLibrary/__init__.py` & `robotframework-xlibrary-2.0.0/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/module1.py` & `robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/module1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from robot.api.deco import keyword
+from robot.api import logger
 from robot.libraries.BuiltIn import BuiltIn
-from AppiumFlutterFinder import FlutterFinder
+from appium_flutter_finder import FlutterFinder
 from AppiumFlutterLibrary import AppiumFlutterLibrary
 from .module2 import XDrint
 import time
 
 class XPrint(AppiumFlutterLibrary):
     def __init__(self):
         super().__init__()
@@ -14,31 +15,30 @@
         self.finder = FlutterFinder()
 
     @keyword("XPrint Log")
     def XPrint_log(self):
         print("Hello, world! เทสภาษาไทย111")
 
     def TestModule2(self):
-        dasdsadsa = XDrint()  # สร้างอินสแตนซ์ของคลาส Module2
-        dasdsadsa.CDCDCD()    # เรียกใช้เมธอด CDCDCD จากอินสแตนซ์นั้น
-        self._ne.CDCDCD()
+        instance = XDrint()  # You might consider renaming the variable to something meaningful
+        instance.CDCDCD()    # Assuming CDCDCD is a valid method
+        self._ne.CDCDCD()    # Ensure that _ne has the method CDCDCD
 
     def XQuit_App(self):
         """ปิดแอพปัจจุบันและปิดเซสชัน"""
         driver = self._current_application()
         driver.quit()
 
-    def Xwitch_Mode(self, mode):
+    @keyword('Switch Mode')
+    def Switch_Mode(self, mode):
         """Switch Mode to NATIVE_APP OR FLUTTER."""
         driver = self._current_application()
-
         if mode == 'NATIVE_APP':
             driver.switch_to.context('NATIVE_APP')
-
-        if mode == 'FLUTTER':
+        elif mode == 'FLUTTER':  # Changed from 'if' to 'elif' for logical correctness
             driver.switch_to.context('FLUTTER')
 
     def _current_application(self):
         """คืนค่าอินสแตนซ์ของแอปพลิเคชันปัจจุบัน"""
         return self._bi.get_library_instance('AppiumFlutterLibrary')._current_application()
 
     @keyword('Is Button Active')
@@ -55,15 +55,14 @@
                 return True
             else:
                 if not is_visible:
                     logger.warn(f"Button with key '{key}' is not visible.")
                 if not is_enabled:
                     logger.warn(f"Button with key '{key}' is not enabled.")
                 return False
-
         except Exception as e:
             logger.error(f"Error checking if button is active: {e}")
             return False
 
     @keyword('Wait Until Button Is Active')
     def wait_until_button_is_active(self, key, timeout=10):
         """Wait until the button with the given key is active in a Flutter application."""
```

### Comparing `robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 1.0.4
+Version: 2.0.0
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

