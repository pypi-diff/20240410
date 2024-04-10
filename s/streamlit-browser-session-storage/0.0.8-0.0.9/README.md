# Comparing `tmp/streamlit-browser-session-storage-0.0.8.tar.gz` & `tmp/streamlit-browser-session-storage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-browser-session-storage-0.0.8.tar", last modified: Wed Apr 10 10:51:17 2024, max compression
+gzip compressed data, was "streamlit-browser-session-storage-0.0.9.tar", last modified: Wed Apr 10 10:57:18 2024, max compression
```

## Comparing `streamlit-browser-session-storage-0.0.8.tar` & `streamlit-browser-session-storage-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 10:51:17.169640 streamlit-browser-session-storage-0.0.8/
--rw-rw-rw-   0        0        0     1082 2023-09-26 20:12:35.000000 streamlit-browser-session-storage-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       70 2023-10-07 22:18:24.000000 streamlit-browser-session-storage-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3630 2024-04-10 10:51:17.164551 streamlit-browser-session-storage-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3315 2024-03-12 16:39:27.000000 streamlit-browser-session-storage-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 10:51:17.169640 streamlit-browser-session-storage-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-04-10 10:50:04.000000 streamlit-browser-session-storage-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 10:51:15.518453 streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/
--rw-rw-rw-   0        0        0     3630 2024-04-10 10:51:12.000000 streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      924 2024-04-10 10:51:14.000000 streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 10:51:12.000000 streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-10 10:51:12.000000 streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-04-10 10:51:12.000000 streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 10:51:15.550289 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/
--rw-rw-rw-   0        0        0     4223 2024-04-10 10:51:06.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/__init__.py
--rw-rw-rw-   0        0        0      391 2024-04-10 10:48:23.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/example.py
-drwxrwxrwx   0        0        0        0 2024-04-10 10:51:15.132246 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-10 10:51:15.945447 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-09-26 20:12:35.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      492 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-10 10:51:15.170699 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-10 10:51:17.137218 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/js/
--rw-rw-rw-   0        0        0   381649 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js
--rw-rw-rw-   0        0        0     1443 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1361006 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.map
+drwxrwxrwx   0        0        0        0 2024-04-10 10:57:18.379570 streamlit-browser-session-storage-0.0.9/
+-rw-rw-rw-   0        0        0     1082 2023-09-26 20:12:35.000000 streamlit-browser-session-storage-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       70 2023-10-07 22:18:24.000000 streamlit-browser-session-storage-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3630 2024-04-10 10:57:18.369423 streamlit-browser-session-storage-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3315 2024-03-12 16:39:27.000000 streamlit-browser-session-storage-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 10:57:18.380565 streamlit-browser-session-storage-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-04-10 10:56:34.000000 streamlit-browser-session-storage-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 10:57:18.077956 streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/
+-rw-rw-rw-   0        0        0     3630 2024-04-10 10:57:15.000000 streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      924 2024-04-10 10:57:16.000000 streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 10:57:15.000000 streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-10 10:57:15.000000 streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-04-10 10:57:15.000000 streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 10:57:18.129091 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/
+-rw-rw-rw-   0        0        0     4319 2024-04-10 10:55:47.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/__init__.py
+-rw-rw-rw-   0        0        0      400 2024-04-10 10:56:54.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/example.py
+drwxrwxrwx   0        0        0        0 2024-04-10 10:57:17.727885 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-10 10:57:18.234565 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-09-26 20:12:35.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      492 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-10 10:57:17.758084 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-10 10:57:18.303470 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   381649 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js
+-rw-rw-rw-   0        0        0     1443 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1361006 2024-04-10 10:50:36.000000 streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.map
```

### Comparing `streamlit-browser-session-storage-0.0.8/LICENSE` & `streamlit-browser-session-storage-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-browser-session-storage-0.0.8/PKG-INFO` & `streamlit-browser-session-storage-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-browser-session-storage
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlit component that allows you to do manage browser session storage
 Home-page: 
 Author: 
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `streamlit-browser-session-storage-0.0.8/README.md` & `streamlit-browser-session-storage-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-browser-session-storage-0.0.8/setup.py` & `streamlit-browser-session-storage-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-browser-session-storage",
-    version="0.0.8",
+    version="0.0.9",
     author="",
     author_email="",
     description="Streamlit component that allows you to do manage browser session storage",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/PKG-INFO` & `streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-browser-session-storage
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlit component that allows you to do manage browser session storage
 Home-page: 
 Author: 
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_browser_session_storage.egg-info/SOURCES.txt` & `streamlit-browser-session-storage-0.0.9/streamlit_browser_session_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/__init__.py` & `streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import ast
 import time
 from typing import Literal, Optional, Union, Any, Dict
 import streamlit as st
 import streamlit.components.v1 as components
 
-_RELEASE = True   
+_RELEASE = False   
  
 if not _RELEASE:
     _st_session_browser_storage = components.declare_component(
 
         "st_session_browser_storage",
 
         url="http://localhost:3001",
@@ -65,15 +65,19 @@
             key: unique identifier for the function/method in case you wish to execute it again somewhere else in the app.
         """
 
         if itemKey is None or itemKey == "":
             return
         
         _st_session_browser_storage(method="deleteItem", itemKey=itemKey, key=key, default=default) 
-        self.storedItems.pop(itemKey) 
+        
+        if itemKey not in self.storedItems: 
+            return
+        else:
+            self.storedItems.pop(itemKey) 
         
     
     def eraseItem(self, itemKey:str, key:str="eraseItem", default=None):
         """
         Erase item from sessionBrowser storage. deleteItem does not remove it from storage, merely changes its default value. This will do so.
 
         Args:
```

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/bootstrap.min.css` & `streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/bootstrap.min.css.map` & `streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js` & `streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js`

 * *Files identical despite different names*

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.LICENSE.txt` & `streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-browser-session-storage-0.0.8/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.map` & `streamlit-browser-session-storage-0.0.9/streamlit_session_browser_storage/frontend/build/static/js/main.44860aa6.js.map`

 * *Files identical despite different names*

