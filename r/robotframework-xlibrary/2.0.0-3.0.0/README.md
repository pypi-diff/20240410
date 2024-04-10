# Comparing `tmp/robotframework-xlibrary-2.0.0.tar.gz` & `tmp/robotframework-xlibrary-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-2.0.0.tar", last modified: Wed Apr 10 02:48:17 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-3.0.0.tar", last modified: Wed Apr 10 03:32:46 2024, max compression
```

## Comparing `robotframework-xlibrary-2.0.0.tar` & `robotframework-xlibrary-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1584 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-10 02:47:01.000000 robotframework-xlibrary-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/XLibrary/
--rw-rw-rw-   0        0        0     1792 2024-04-09 09:39:59.000000 robotframework-xlibrary-2.0.0/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-2.0.0/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     3136 2024-04-10 02:46:51.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-2.0.0/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     1584 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-10 02:48:17.000000 robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1584 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-3.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-04-10 03:32:33.000000 robotframework-xlibrary-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/XLibrary/
+-rw-rw-rw-   0        0        0     1792 2024-04-09 09:39:59.000000 robotframework-xlibrary-3.0.0/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-3.0.0/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     3246 2024-04-10 03:31:51.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-3.0.0/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     1584 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 03:32:46.000000 robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-2.0.0/PKG-INFO` & `robotframework-xlibrary-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 2.0.0
+Version: 3.0.0
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-2.0.0/README.md` & `robotframework-xlibrary-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-2.0.0/setup.py` & `robotframework-xlibrary-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="2.0.0",
+    version="3.0.0",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Test Library for robotframework-xlibrary",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-2.0.0/src/XLibrary/__init__.py` & `robotframework-xlibrary-3.0.0/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-2.0.0/src/XLibrary/submodule1/module1.py` & `robotframework-xlibrary-3.0.0/src/XLibrary/submodule1/module1.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,17 @@
         """คืนค่าอินสแตนซ์ของแอปพลิเคชันปัจจุบัน"""
         return self._bi.get_library_instance('AppiumFlutterLibrary')._current_application()
 
     @keyword('Is Button Active')
     def is_button_active(self, key):
         """Check if the button with the given key is active in a Flutter application."""
         try:
+            driver = self._current_application() #มีการเพิ่มเข้ามา
             button = self.finder.by_value_key(key)
-            element = self.driver.find_element(button)
+            element = driver.find_element(button)   #ลบ self
             is_visible = element.is_displayed()
             is_enabled = element.is_enabled()
 
             if is_visible and is_enabled:
                 logger.info(f"Button with key '{key}' is active and visible.")
                 return True
             else:
```

### Comparing `robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 2.0.0
+Version: 3.0.0
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-2.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-3.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

