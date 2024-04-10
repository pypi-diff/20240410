# Comparing `tmp/qaml-0.0.6.tar.gz` & `tmp/qaml-0.0.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.6.tar", last modified: Wed Apr 10 16:49:00 2024, max compression
+gzip compressed data, was "qaml-0.0.6.post1.tar", last modified: Wed Apr 10 17:14:20 2024, max compression
```

## Comparing `qaml-0.0.6.tar` & `qaml-0.0.6.post1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 16:49:00.925164 qaml-0.0.6/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.6/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      717 2024-04-10 16:49:00.925015 qaml-0.0.6/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      172 2024-04-10 16:48:11.000000 qaml-0.0.6/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-10 16:48:43.000000 qaml-0.0.6/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 16:49:00.924182 qaml-0.0.6/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.6/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      852 2024-04-08 20:17:36.000000 qaml-0.0.6/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    10069 2024-04-10 16:48:11.000000 qaml-0.0.6/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 16:49:00.924864 qaml-0.0.6/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      717 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-10 16:49:00.000000 qaml-0.0.6/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-10 16:49:00.925197 qaml-0.0.6/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 17:14:20.734454 qaml-0.0.6.post1/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.6.post1/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      723 2024-04-10 17:14:20.734311 qaml-0.0.6.post1/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      172 2024-04-10 16:48:11.000000 qaml-0.0.6.post1/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-10 17:14:00.000000 qaml-0.0.6.post1/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 17:14:20.733372 qaml-0.0.6.post1/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.6.post1/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      852 2024-04-08 20:17:36.000000 qaml-0.0.6.post1/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    10006 2024-04-10 17:13:19.000000 qaml-0.0.6.post1/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 17:14:20.734147 qaml-0.0.6.post1/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      723 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-10 17:14:20.734495 qaml-0.0.6.post1/setup.cfg
```

### Comparing `qaml-0.0.6/LICENSE` & `qaml-0.0.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.6/PKG-INFO` & `qaml-0.0.6.post1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.6
+Version: 0.0.6.post1
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.6/pyproject.toml` & `qaml-0.0.6.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.6"
+version = "0.0.6-1"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.6/qaml/__main__.py` & `qaml-0.0.6.post1/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.6/qaml/client.py` & `qaml-0.0.6.post1/qaml/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,15 @@
     def report_error(self, reason):
         raise QAMLExecException(reason)
 
     def set_context(self, context):
         self.context = context
 
     def get_screenshot(self):
-        start_time = time.time()
         screenshot = self.driver.get_screenshot_as_base64()
-        print(f"Screenshot took {time.time() - start_time} seconds.")
         PIL_image = Image.open(BytesIO(base64.b64decode(screenshot)))
         longer_side = max(PIL_image.size)
         aspect_ratio = PIL_image.size[0] / PIL_image.size[1]
         new_size = (960, int(960 / aspect_ratio)) if PIL_image.size[0] == longer_side else (int(960 * aspect_ratio), 960)
         PIL_image = PIL_image.resize(new_size)
         buffered = BytesIO()
         PIL_image.save(buffered, format="PNG")
@@ -163,15 +161,16 @@
             # try 3 times to setup the driver
             for _ in range(3):
                 try:
                     self.setup_driver(ios_udid)
                     break
                 except:
                     pass
-            else:
+            else Exception as e:
+                print(e)
                 raise Exception("Failed to setup the driver.")
         self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self, udid):
         options = XCUITestOptions()
         options.udid = udid
         custom_caps = {"mjpegScreenshotUrl": "http://localhost:9100"}
```

### Comparing `qaml-0.0.6/qaml.egg-info/PKG-INFO` & `qaml-0.0.6.post1/qaml.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.6
+Version: 0.0.6.post1
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

