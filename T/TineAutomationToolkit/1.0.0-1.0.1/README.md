# Comparing `tmp/TineAutomationToolkit-1.0.0.tar.gz` & `tmp/TineAutomationToolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TineAutomationToolkit-1.0.0.tar", last modified: Tue Mar 19 04:36:37 2024, max compression
+gzip compressed data, was "dist\TineAutomationToolkit-1.0.1.tar", last modified: Wed Apr 10 08:20:52 2024, max compression
```

## Comparing `TineAutomationToolkit-1.0.0.tar` & `TineAutomationToolkit-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/
--rw-rw-rw-   0        0        0     2280 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/
--rw-rw-rw-   0        0        0      356 2024-03-19 04:35:22.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/
--rw-rw-rw-   0        0        0      587 2024-03-19 04:35:08.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/capturescreenshot.py
--rw-rw-rw-   0        0        0     3404 2024-03-19 02:55:10.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/connectionmanagement.py
--rw-rw-rw-   0        0        0     9730 2024-03-19 02:58:49.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/controlelement.py
--rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/scroll.py
--rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/toolkitstest.py
--rw-rw-rw-   0        0        0     5899 2024-03-19 02:59:09.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/waitingelement.py
-drwxrwxrwx   0        0        0        0 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 04:36:37.000000 TineAutomationToolkit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-03-19 04:34:30.000000 TineAutomationToolkit-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/
+-rw-rw-rw-   0        0        0     2280 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/
+-rw-rw-rw-   0        0        0      356 2024-03-19 04:35:22.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/
+-rw-rw-rw-   0        0        0      587 2024-03-19 04:35:08.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/capturescreenshot.py
+-rw-rw-rw-   0        0        0     3404 2024-04-09 05:36:45.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/connectionmanagement.py
+-rw-rw-rw-   0        0        0    11728 2024-04-10 08:17:33.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/controlelement.py
+-rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/scroll.py
+-rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/toolkitstest.py
+-rw-rw-rw-   0        0        0     5899 2024-03-19 02:59:09.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/waitingelement.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 08:20:52.000000 TineAutomationToolkit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-04-10 02:35:56.000000 TineAutomationToolkit-1.0.1/setup.py
```

### Comparing `TineAutomationToolkit-1.0.0/PKG-INFO` & `TineAutomationToolkit-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.0/README.md` & `TineAutomationToolkit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/__init__.py` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/capturescreenshot.py` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/capturescreenshot.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/connectionmanagement.py` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/connectionmanagement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/controlelement.py` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/controlelement.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 import ast
 
 from AppiumLibrary.locators import ElementFinder
 from AppiumLibrary.keywords._logging import _LoggingKeywords
 from .connectionmanagement import ConnectionManagement
 from selenium.webdriver.remote.webelement import WebElement
 from appium.webdriver.common.touch_action import TouchAction
+from TineAutomationToolkit.detect.detectelement import DetectElement
+from TineAutomationToolkit.detect import detectelement
 
 
 cache_app = ConnectionManagement()
 log = _LoggingKeywords()
 element_finder_t = ElementFinder()
-
+detect_element_finder = DetectElement()
+test = detectelement()
 
 def isstr(s):
     return isinstance(s, str)
 
 
 class ControlElement:
 
@@ -189,15 +192,59 @@
         ตัวอย่างการใช้งาน:
 
         | t_input_text | ข้อความที่ต้องการจะใส่ |
 
         """
         log._info("Typing text '%s' into text field '%s'" % (text, locator))
         self._element_input_text_by_locator(locator, text)
+
+    def flutter_get_element_attribute(self, locator, attribute):
+        """Get element attribute using given attribute: name, value,...
+
+        Examples:
+
+        | Get Element Attribute | locator | name |
+        | Get Element Attribute | locator | value |
+        """
+        elements = self._element_find_flutter(locator, False, True)
+        # elements = self._element_find_t(locator, False, True)
+        ele_len = len(elements)
+        if ele_len == 0:
+            raise AssertionError("Element '%s' could not be found" % locator)
+        elif ele_len > 1:
+            self._info("CAUTION: '%s' matched %s elements - using the first element only" % (locator, len(elements)))
+
+        try:
+            attr_val = elements[0].get_attribute(attribute)
+            log._info("Element '%s' attribute '%s' value '%s' " % (locator, attribute, attr_val))
+            return attr_val
+        except:
+            raise AssertionError("Attribute '%s' is not valid for element '%s'" % (attribute, locator))
+    
     #PRIVATE_FUNCTION
+
+    def _element_find_flutter(self, locator, first_only, required, tag=None):
+        application = cache_app._current_application()
+        elements = None
+        if isstr(locator):
+            _locator = locator
+            element = detect_element_finder.find_attribute(application , _locator , tag)
+            if required and len(elements) == 0:
+                raise ValueError("Element locator '" + locator + "' did not match any elements.")
+            if first_only:
+                if len(elements) == 0: return None
+                return elements[0]
+        elif isinstance(locator, WebElement):
+            if first_only:
+                return locator
+            else:
+                elements = [locator]
+
+        
+        return element
         
     def _element_find_t(self, locator, first_only, required, tag=None):
         application = cache_app._current_application()
         elements = None
         if isstr(locator):
             _locator = locator
             elements = element_finder_t.find(application, _locator, tag)
```

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/scroll.py` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/scroll.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit/keywords/waitingelement.py` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit/keywords/waitingelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/PKG-INFO` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.0/TineAutomationToolkit.egg-info/SOURCES.txt` & `TineAutomationToolkit-1.0.1/TineAutomationToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.0/setup.py` & `TineAutomationToolkit-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="TineAutomationToolkit",
-    version="1.0.0",
+    version="1.0.1",
     author="Pornpawit Suttha",
     author_email="pornpawit14suttha@gmail.com",
     description="Test Library for TineAutomationToolkit",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pornpawit08/TineAutomationToolkit.git",
     packages=find_packages(),
```

