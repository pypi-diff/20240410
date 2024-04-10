# Comparing `tmp/qaml-0.0.5.tar.gz` & `tmp/qaml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.5.tar", last modified: Mon Apr  8 19:51:41 2024, max compression
+gzip compressed data, was "qaml-0.0.6.tar", last modified: Wed Apr 10 16:49:00 2024, max compression
```

## Comparing `qaml-0.0.5.tar` & `qaml-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-08 19:51:41.820960 qaml-0.0.5/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.5/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-08 19:51:41.820815 qaml-0.0.5/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       74 2024-04-02 18:28:00.000000 qaml-0.0.5/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-08 19:46:35.000000 qaml-0.0.5/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-08 19:51:41.819912 qaml-0.0.5/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.5/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      852 2024-04-08 19:47:07.000000 qaml-0.0.5/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     8465 2024-04-08 19:50:04.000000 qaml-0.0.5/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-08 19:51:41.820668 qaml-0.0.5/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-08 19:51:41.820990 qaml-0.0.5/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 16:49:00.925164 qaml-0.0.6/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.6/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      717 2024-04-10 16:49:00.925015 qaml-0.0.6/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      172 2024-04-10 16:48:11.000000 qaml-0.0.6/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-10 16:48:43.000000 qaml-0.0.6/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 16:49:00.924182 qaml-0.0.6/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.6/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      852 2024-04-08 20:17:36.000000 qaml-0.0.6/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    10069 2024-04-10 16:48:11.000000 qaml-0.0.6/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 16:49:00.924864 qaml-0.0.6/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      717 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-10 16:49:00.925197 qaml-0.0.6/setup.cfg
```

### Comparing `qaml-0.0.5/LICENSE` & `qaml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.5/pyproject.toml` & `qaml-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.5/qaml/__main__.py` & `qaml-0.0.6/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.5/qaml/client.py` & `qaml-0.0.6/qaml/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 import time
 import base64
 import subprocess
 import json
 from PIL import Image
 from io import BytesIO
 import requests
+import os
 
 class QAMLExecException(Exception):
     pass
 
 class BaseClient:
     def __init__(self, api_key):
-        self.api_key = api_key
+        self.api_key = api_key or os.environ.get("QAML_API_KEY")
         self.driver = None
         self.platform = None
         self.screen_size = None
+        self.req_session = requests.Session()
+        self.req_session.headers.update({"Authorization": f"Bearer {api_key}"})
+        self.context = ''
 
     def setup_driver(self):
         raise NotImplementedError
 
     def tap_coordinates(self, x, y):
         raise NotImplementedError
 
@@ -41,26 +45,35 @@
 
     def sleep(self, duration):
         time.sleep(duration)
 
     def report_error(self, reason):
         raise QAMLExecException(reason)
 
-    def execute(self, script):
+    def set_context(self, context):
+        self.context = context
+
+    def get_screenshot(self):
+        start_time = time.time()
         screenshot = self.driver.get_screenshot_as_base64()
+        print(f"Screenshot took {time.time() - start_time} seconds.")
         PIL_image = Image.open(BytesIO(base64.b64decode(screenshot)))
         longer_side = max(PIL_image.size)
         aspect_ratio = PIL_image.size[0] / PIL_image.size[1]
         new_size = (960, int(960 / aspect_ratio)) if PIL_image.size[0] == longer_side else (int(960 * aspect_ratio), 960)
         PIL_image = PIL_image.resize(new_size)
         buffered = BytesIO()
         PIL_image.save(buffered, format="PNG")
         screenshot = base64.b64encode(buffered.getvalue()).decode("utf-8")
-        payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot}
-        response = requests.post("https://api.camelqa.com/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
+        return screenshot
+
+    def execute(self, script):
+        screenshot = self.get_screenshot()
+        payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.context}
+        response = self.req_session.post("https://api.camelqa.com/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(response.text)
         actions = response.json()
         available_functions = {
             "tap": self.tap_coordinates,
             "drag": self.drag,
             "swipe": self.swipe,
             "scroll": self.scroll,
@@ -70,14 +83,20 @@
             "switch_to_app": self.switch_to_app,
         }
         for action in actions:
             function = available_functions[action["name"]]
             arguments = json.loads(action["arguments"])
             function(**arguments)
 
+    def agent(self, task):
+        screenshot = self.get_screenshot()
+        payload = {"task": task, "platform": self.platform, "screenshot": screenshot}
+        response = self.req_session.post("https://api.camelqa.com/v1/agent", json=payload)
+        print(response.text)
+
 class AndroidClient(BaseClient):
     def __init__(self, api_key, driver=None):
         super().__init__(api_key)
         self.platform = "Android"
         if driver:
             self.driver = driver
         else:
@@ -91,15 +110,28 @@
                 raise Exception("Failed to setup the driver.")
         self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self):
         caps = {'deviceName': 'Android Device', 'automationName': 'UiAutomator2', 'autoGrantPermissions': True,
                 'newCommandTimeout': 600, 'mjpegScreenshotUrl': "http://localhost:4723/stream.mjpeg"}
         options = UiAutomator2Options().load_capabilities(caps)
-        self.driver = webdriver.Remote('http://localhost:4723', options=options)
+
+        def create_driver(options):
+            try:
+                return webdriver.Remote('http://localhost:4723', options=options)
+            except:
+                return webdriver.Remote('http://localhost:4723/wd/hub', options=options)
+        try:
+            self.driver = webdriver.Remote('http://localhost:4723', options=options)
+        except:
+            # Try again without mjpeg-consumer dependency
+            caps.pop('mjpegScreenshotUrl')
+            options = UiAutomator2Options().load_capabilities(caps)
+            self.driver = create_driver(options)
+
         self.driver.start_recording_screen()
         self.driver.update_settings({'waitForIdleTimeout': 0, 'shouldWaitForQuiescence': False, 'maxTypingFrequency': 60})
         # get screenshot to test if the driver is working
         self.driver.get_screenshot_as_base64()
 
     def tap_coordinates(self, x, y):
         self.driver.tap([(x, y)], 1)
@@ -140,18 +172,28 @@
         self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self, udid):
         options = XCUITestOptions()
         options.udid = udid
         custom_caps = {"mjpegScreenshotUrl": "http://localhost:9100"}
         options.load_capabilities(custom_caps)
+
+        def create_driver(options):
+            try:
+                return webdriver.Remote('http://localhost:4723', options=options)
+            except:
+                return webdriver.Remote('http://localhost:4723/wd/hub', options=options)
         try:
-            self.driver = webdriver.Remote('http://localhost:4723', options=options)
+            self.driver = create_driver(options)
         except:
-            self.driver = webdriver.Remote('http://localhost:4723/wd/hub', options=options)
+            # Try again without mjpeg-consumer dependency
+            options = XCUITestOptions()
+            options.udid = udid
+            self.driver = create_driver(options)
+
         self.driver.start_recording_screen(forceRestart=True)
         self.driver.update_settings({'waitForIdleTimeout': 0, 'shouldWaitForQuiescence': False, 'maxTypingFrequency': 60})
         # get screenshot to test if the driver is working
         self.driver.get_screenshot_as_base64()
 
     def tap_coordinates(self, x, y):
         self.driver.execute_script("mobile: tap", {"x": x, "y": y})
```

