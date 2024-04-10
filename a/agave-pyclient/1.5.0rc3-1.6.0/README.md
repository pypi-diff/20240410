# Comparing `tmp/agave_pyclient-1.5.0rc3.tar.gz` & `tmp/agave_pyclient-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agave_pyclient-1.5.0rc3.tar", last modified: Tue May  2 19:53:22 2023, max compression
+gzip compressed data, was "agave_pyclient-1.6.0.tar", last modified: Wed Apr 10 16:34:27 2024, max compression
```

## Comparing `agave_pyclient-1.5.0rc3.tar` & `agave_pyclient-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/agave_pyclient/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/agave_pyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/agave_pyclient/agave.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/agave_pyclient/commandbuffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/agave_renderer.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5384 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 19:53:22.739859 agave_pyclient-1.5.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:27.396143 agave_pyclient-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-10 16:34:27.396143 agave_pyclient-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:27.396143 agave_pyclient-1.6.0/agave_pyclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/agave_pyclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30183 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/agave_pyclient/agave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/agave_pyclient/commandbuffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:27.396143 agave_pyclient-1.6.0/agave_pyclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-10 16:34:27.000000 agave_pyclient-1.6.0/agave_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-10 16:34:27.000000 agave_pyclient-1.6.0/agave_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:34:27.000000 agave_pyclient-1.6.0/agave_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:34:27.000000 agave_pyclient-1.6.0/agave_pyclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-10 16:34:27.000000 agave_pyclient-1.6.0/agave_pyclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 16:34:27.000000 agave_pyclient-1.6.0/agave_pyclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:27.396143 agave_pyclient-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/docs/agave_renderer.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5379 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-10 16:34:27.396143 agave_pyclient-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-10 16:34:20.000000 agave_pyclient-1.6.0/setup.py
```

### Comparing `agave_pyclient-1.5.0rc3/CONTRIBUTING.md` & `agave_pyclient-1.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc3/LICENSE` & `agave_pyclient-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc3/PKG-INFO` & `agave_pyclient-1.6.0/agave_pyclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: agave_pyclient
-Version: 1.5.0rc3
+Name: agave-pyclient
+Version: 1.6.0
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
@@ -29,40 +28,40 @@
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # agave_pyclient
 
-A Python client for the Agave 3d volume renderer
+A Python client for the AGAVE 3d volume renderer
 
 ---
 
 ## Features
 
-- Connects to Agave server and sends draw commands. Receives and saves rendered images.
+- Connects to AGAVE server and sends draw commands. Receives and saves rendered images.
 
 ## Quick Start
 
-You must have Agave installed. On command line, run:
+You must have AGAVE installed. On command line, run:
 
 ```
 agave --server &
 ```
 
 For Linux headless operation, you need to tell the Qt library to use the offscreen platform plugin:
 
 ```
 agave -platform offscreen --server &
 ```
 
 ```python
 from agave_pyclient import AgaveRenderer
 
-# 1. connect to the agave server
+# 1. connect to the AGAVE server
 r = agave_pyclient.AgaveRenderer()
 # 2. tell it what data to load
 r.load_data("my_favorite.ome.tiff")
 # 3. set some render settings (abbreviated list here)
 r.set_resolution(681, 612)
 r.background_color(0, 0, 0)
 r.render_iterations(128)
@@ -108,9 +107,7 @@
 
 4. `make docs`
 
    This will generate and launch a web browser to view the most up-to-date
    documentation for your Python package.
 
 **Allen Institute Software License**
-
-
```

### Comparing `agave_pyclient-1.5.0rc3/README.md` & `agave_pyclient-1.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # agave_pyclient
 
-A Python client for the Agave 3d volume renderer
+A Python client for the AGAVE 3d volume renderer
 
 ---
 
 ## Features
 
-- Connects to Agave server and sends draw commands. Receives and saves rendered images.
+- Connects to AGAVE server and sends draw commands. Receives and saves rendered images.
 
 ## Quick Start
 
-You must have Agave installed. On command line, run:
+You must have AGAVE installed. On command line, run:
 
 ```
 agave --server &
 ```
 
 For Linux headless operation, you need to tell the Qt library to use the offscreen platform plugin:
 
 ```
 agave -platform offscreen --server &
 ```
 
 ```python
 from agave_pyclient import AgaveRenderer
 
-# 1. connect to the agave server
+# 1. connect to the AGAVE server
 r = agave_pyclient.AgaveRenderer()
 # 2. tell it what data to load
 r.load_data("my_favorite.ome.tiff")
 # 3. set some render settings (abbreviated list here)
 r.set_resolution(681, 612)
 r.background_color(0, 0, 0)
 r.render_iterations(128)
```

### Comparing `agave_pyclient-1.5.0rc3/agave_pyclient/agave.py` & `agave_pyclient-1.6.0/agave_pyclient/agave.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,26 +151,35 @@
 
 
 class AgaveRenderer:
     """
     AgaveRenderer communicates with AGAVE running in server mode to perform GPU volume
     rendering.
 
+    Parameters
+    ----------
+    url: str
+        Full url to websocket server including port
+    mode: str
+        "pathtrace" or "raymarch" (pathtrace is default)
+
     Examples
     --------
     Connect to an already running local AGAVE server instance
 
     >>> agaveclient = AgaveRenderer()
 
     """
 
-    def __init__(self) -> None:
+    def __init__(self, url="ws://localhost:1235/", mode="pathtrace") -> None:
         self.cb = CommandBuffer()
         self.session_name = ""
-        self.ws = AgaveClient("ws://localhost:1235/", protocols=["http-only", "chat"])
+        if mode != "pathtrace" and mode != "raymarch":
+            mode = "pathtrace"
+        self.ws = AgaveClient(f"{url}?mode={mode}", protocols=["http-only", "chat"])
         # self.ws.onOpened = self.onOpen
         self.ws.connect()
         # self.ws.run_forever()
         # except KeyboardInterrupt:
         #     print("keyboard")
         #     ws.close()
 
@@ -896,14 +905,26 @@
             Any list length other than 0 or 6 is an error.
         """
         # 44
         self.cb.add_command(
             "LOAD_DATA", path, scene, multiresolution_level, time, channels, region
         )
 
+    def show_scale_bar(self, on: int):
+        """
+        Turn scale bar display on or off
+
+        Parameters
+        ----------
+        on: int
+            0 to hide scale bar, 1 to show it
+        """
+        # 45
+        self.cb.add_command("SHOW_SCALE_BAR", on)
+
     def batch_render_turntable(
         self, number_of_frames=90, direction=1, output_name="frame", first_frame=0
     ):
         """
         Loop to render a turntable sequence, a 360 degree rotation about the vertical
         axis.  Other commands must have been previously issued to load the data and set
         all the viewing parameters.
```

### Comparing `agave_pyclient-1.5.0rc3/agave_pyclient/commandbuffer.py` & `agave_pyclient-1.6.0/agave_pyclient/commandbuffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     # causes data to be loaded
     "SET_TIME": [40, "I32"],
     "SET_BOUNDING_BOX_COLOR": [41, "F32", "F32", "F32"],
     "SHOW_BOUNDING_BOX": [42, "I32"],
     "TRACKBALL_CAMERA": [43, "F32", "F32"],
     # path, scene, multiresolution level, t, channel indices, region
     "LOAD_DATA": [44, "S", "I32", "I32", "I32", "I32A", "I32A"],
+    "SHOW_SCALE_BAR": [45, "I32"],
 }
 
 
 # strategy: add elements to prebuffer,
 # and then traverse prebuffer to convert to binary before sending?
 class CommandBuffer:
     def __init__(self, command_list=None):
```

### Comparing `agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/PKG-INFO` & `agave_pyclient-1.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: agave-pyclient
-Version: 1.5.0rc3
+Name: agave_pyclient
+Version: 1.6.0
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
@@ -29,40 +28,40 @@
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # agave_pyclient
 
-A Python client for the Agave 3d volume renderer
+A Python client for the AGAVE 3d volume renderer
 
 ---
 
 ## Features
 
-- Connects to Agave server and sends draw commands. Receives and saves rendered images.
+- Connects to AGAVE server and sends draw commands. Receives and saves rendered images.
 
 ## Quick Start
 
-You must have Agave installed. On command line, run:
+You must have AGAVE installed. On command line, run:
 
 ```
 agave --server &
 ```
 
 For Linux headless operation, you need to tell the Qt library to use the offscreen platform plugin:
 
 ```
 agave -platform offscreen --server &
 ```
 
 ```python
 from agave_pyclient import AgaveRenderer
 
-# 1. connect to the agave server
+# 1. connect to the AGAVE server
 r = agave_pyclient.AgaveRenderer()
 # 2. tell it what data to load
 r.load_data("my_favorite.ome.tiff")
 # 3. set some render settings (abbreviated list here)
 r.set_resolution(681, 612)
 r.background_color(0, 0, 0)
 r.render_iterations(128)
@@ -108,9 +107,7 @@
 
 4. `make docs`
 
    This will generate and launch a web browser to view the most up-to-date
    documentation for your Python package.
 
 **Allen Institute Software License**
-
-
```

### Comparing `agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/requires.txt` & `agave_pyclient-1.6.0/agave_pyclient.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 numpy
 ws4py==0.5.1
-Pillow==9.3.0
+Pillow==10.2.0
 
 [all]
 numpy
 ws4py==0.5.1
-Pillow==9.3.0
+Pillow==10.2.0
 pytest-runner>=5.2
 black>=19.10b0
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
 ipython>=7.15.0
 m2r2>=0.2.7
-pytest-runner>=5.2
 Sphinx>=3.4.3
 sphinx_rtd_theme>=0.5.1
 tox>=3.15.2
 twine>=3.1.1
 wheel>=0.34.2
 
 [dev]
@@ -32,15 +31,14 @@
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
 ipython>=7.15.0
 m2r2>=0.2.7
-pytest-runner>=5.2
 Sphinx>=3.4.3
 sphinx_rtd_theme>=0.5.1
 tox>=3.15.2
 twine>=3.1.1
 wheel>=0.34.2
 
 [setup]
```

### Comparing `agave_pyclient-1.5.0rc3/docs/Makefile` & `agave_pyclient-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc3/docs/conf.py` & `agave_pyclient-1.6.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 author = u"Daniel Toloudis"
 
 # The version info for the project you"re documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The full version, including alpha/beta/rc tags
-release = "1.5.0-rc.3"
+release = "1.6.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `agave_pyclient-1.5.0rc3/docs/index.rst` & `agave_pyclient-1.6.0/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 And then in your Python code, import and use the :ref:`agave-renderer-label` class.
 
 .. code-block:: python
 
    from agave_pyclient import AgaveRenderer
 
-   # 1. connect to the agave server
+   # 1. connect to the AGAVE server
    r = agave_pyclient.AgaveRenderer()
    # 2. tell it what data to load
    r.load_data("my_favorite.ome.tiff", 0, 0, 0, [], [])
    # 3. set some render settings (abbreviated list here)
    r.set_resolution(681, 612)
    r.background_color(0, 0, 0)
    r.render_iterations(128)
```

### Comparing `agave_pyclient-1.5.0rc3/docs/make.bat` & `agave_pyclient-1.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc3/setup.py` & `agave_pyclient-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Sphinx>=3.4.3",
     "sphinx_rtd_theme>=0.5.1",
     "tox>=3.15.2",
     "twine>=3.1.1",
     "wheel>=0.34.2",
 ]
 
-requirements = ["numpy", "ws4py==0.5.1", "Pillow==9.3.0"]
+requirements = ["numpy", "ws4py==0.5.1", "Pillow==10.2.0"]
 
 extra_requirements = {
     "setup": setup_requirements,
     "test": test_requirements,
     "dev": dev_requirements,
     "all": [*requirements, *dev_requirements,],
 }
@@ -79,10 +79,10 @@
     setup_requires=setup_requirements,
     test_suite="agave_pyclient/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/allen-cell-animated/agave",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="1.5.0-rc.3",
+    version="1.6.0",
     zip_safe=False,
 )
```

