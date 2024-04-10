# Comparing `tmp/pyxl30-tspspi-0.0.7.tar.gz` & `tmp/pyxl30-tspspi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxl30-tspspi-0.0.7.tar", last modified: Tue Apr  2 16:16:34 2024, max compression
+gzip compressed data, was "pyxl30-tspspi-0.0.8.tar", last modified: Wed Apr 10 13:48:38 2024, max compression
```

## Comparing `pyxl30-tspspi-0.0.7.tar` & `pyxl30-tspspi-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.137574 pyxl30-tspspi-0.0.7/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1410 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/LICENSE.md
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2588 2024-04-02 16:16:34.137519 pyxl30-tspspi-0.0.7/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2049 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/README.md
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      183 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/pyproject.toml
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      652 2024-04-02 16:16:34.138064 pyxl30-tspspi-0.0.7/setup.cfg
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.134713 pyxl30-tspspi-0.0.7/src/
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.137236 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2588 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      350 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)        1 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)       39 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)       11 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.136954 pyxl30-tspspi-0.0.7/src/xl30serial/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/src/xl30serial/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)    10020 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/src/xl30serial/scanningelectronmicroscope.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)    56070 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/src/xl30serial/xl30serial.py
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-10 13:48:38.973721 pyxl30-tspspi-0.0.8/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1410 2024-04-10 13:48:24.000000 pyxl30-tspspi-0.0.8/LICENSE.md
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2588 2024-04-10 13:48:38.973672 pyxl30-tspspi-0.0.8/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2049 2024-04-10 13:48:24.000000 pyxl30-tspspi-0.0.8/README.md
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      183 2024-04-10 13:48:24.000000 pyxl30-tspspi-0.0.8/pyproject.toml
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      652 2024-04-10 13:48:38.974172 pyxl30-tspspi-0.0.8/setup.cfg
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-10 13:48:38.971056 pyxl30-tspspi-0.0.8/src/
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-10 13:48:38.973436 pyxl30-tspspi-0.0.8/src/pyxl30_tspspi.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2588 2024-04-10 13:48:38.000000 pyxl30-tspspi-0.0.8/src/pyxl30_tspspi.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      350 2024-04-10 13:48:38.000000 pyxl30-tspspi-0.0.8/src/pyxl30_tspspi.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)        1 2024-04-10 13:48:38.000000 pyxl30-tspspi-0.0.8/src/pyxl30_tspspi.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)       39 2024-04-10 13:48:38.000000 pyxl30-tspspi-0.0.8/src/pyxl30_tspspi.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)       11 2024-04-10 13:48:38.000000 pyxl30-tspspi-0.0.8/src/pyxl30_tspspi.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-10 13:48:38.973183 pyxl30-tspspi-0.0.8/src/xl30serial/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-10 13:48:24.000000 pyxl30-tspspi-0.0.8/src/xl30serial/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    10020 2024-04-10 13:48:24.000000 pyxl30-tspspi-0.0.8/src/xl30serial/scanningelectronmicroscope.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    56640 2024-04-10 13:48:24.000000 pyxl30-tspspi-0.0.8/src/xl30serial/xl30serial.py
```

### Comparing `pyxl30-tspspi-0.0.7/LICENSE.md` & `pyxl30-tspspi-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxl30-tspspi-0.0.7/PKG-INFO` & `pyxl30-tspspi-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxl30-tspspi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Control libraries and utilities for the XL30 ESEM (unofficial)
 Home-page: https://github.com/tspspi/pyxl30
 Author: Thomas Spielauer
 Author-email: pypipackages01@tspi.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxl30-tspspi-0.0.7/README.md` & `pyxl30-tspspi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyxl30-tspspi-0.0.7/setup.cfg` & `pyxl30-tspspi-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/PKG-INFO` & `pyxl30-tspspi-0.0.8/src/pyxl30_tspspi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxl30-tspspi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Control libraries and utilities for the XL30 ESEM (unofficial)
 Home-page: https://github.com/tspspi/pyxl30
 Author: Thomas Spielauer
 Author-email: pypipackages01@tspi.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxl30-tspspi-0.0.7/src/xl30serial/scanningelectronmicroscope.py` & `pyxl30-tspspi-0.0.8/src/xl30serial/scanningelectronmicroscope.py`

 * *Files identical despite different names*

### Comparing `pyxl30-tspspi-0.0.7/src/xl30serial/xl30serial.py` & `pyxl30-tspspi-0.0.8/src/xl30serial/xl30serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,34 @@
     def __call__(self, func):
         def wrapper(*args, **kwargs):
             args[0]._logger.warning(f"Calling function {func} with known bugs ({self._bugs})!")
             return func(*args, **kwargs)
         return wrapper
 
 class XL30(ScanningElectronMicroscope):
+    super().__init__(
+        highTension = (100, 30e3),
+        spotSize = (1, 10),
+        magnification = (10, 100000),
+        supportedScanModes = [
+            ScanningElectronMicroscope_ScanMode.FULL_FRAME,
+            ScanningElectronMicroscope_ScanMode.SELECTED_AREA,
+            ScanningElectronMicroscope_ScanMode.SPOT,
+            ScanningElectronMicroscope_ScanMode.LINE_X,
+            ScanningElectronMicroscope_ScanMode.LINE_Y,
+            ScanningElectronMicroscope_ScanMode.EXT_XY
+        ],
+        stigmatorCount = 1
+    )
     pass
 
 class XL30Serial(XL30):
     def __init__(self, port, logger = None, debug = False, loglevel = "ERROR", detectorsAutodetect = False, retryCount = 3, reconnectCount = 3, retryDelay = 5, reconnectDelay = 5):
+        super().__init__()
+
         self._retryCount = retryCount
         self._reconnectCount = reconnectCount
 
         self._retryCountState = retryCount
         self._reconnectCountState = reconnectCount
 
         self._retryDelay = retryDelay
```

