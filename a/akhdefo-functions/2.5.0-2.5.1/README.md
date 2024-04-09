# Comparing `tmp/akhdefo_functions-2.5.0.tar.gz` & `tmp/akhdefo_functions-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akhdefo_functions-2.5.0.tar", last modified: Sun Apr  7 01:02:18 2024, max compression
+gzip compressed data, was "akhdefo_functions-2.5.1.tar", last modified: Tue Apr  9 22:07:06 2024, max compression
```

## Comparing `akhdefo_functions-2.5.0.tar` & `akhdefo_functions-2.5.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 01:02:18.512036 akhdefo_functions-2.5.0/
--rw-rw-rw-   0        0        0     3935 2024-04-07 01:02:18.511031 akhdefo_functions-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2673 2024-03-16 00:59:39.000000 akhdefo_functions-2.5.0/README_pypi.md
-drwxrwxrwx   0        0        0        0 2024-04-07 01:02:18.499527 akhdefo_functions-2.5.0/akhdefo_functions/
--rw-rw-rw-   0        0        0    53386 2024-04-07 00:24:07.000000 akhdefo_functions-2.5.0/akhdefo_functions/AkhdefoPlot.py
--rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Classification.py
--rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Coreg.py
--rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_GOI.py
--rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_TS.py
--rw-rw-rw-   0        0        0    76847 2024-04-06 22:26:04.000000 akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Tools.py
--rw-rw-rw-   0        0        0   153494 2024-04-06 23:34:54.000000 akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Utilities.py
--rw-rw-rw-   0        0        0    27026 2024-04-07 00:07:47.000000 akhdefo_functions-2.5.0/akhdefo_functions/Filter_PreProc.py
--rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.0/akhdefo_functions/Mosaic_Crop.py
--rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.0/akhdefo_functions/OpticalFlow.py
--rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.0/akhdefo_functions/Stacked_Velocity.py
--rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.0/akhdefo_functions/Unzip_CopyFiles.py
--rw-rw-rw-   0        0        0     9247 2024-04-06 23:49:30.000000 akhdefo_functions-2.5.0/akhdefo_functions/Video_Streamer.py
--rw-rw-rw-   0        0        0      683 2024-04-07 00:41:55.000000 akhdefo_functions-2.5.0/akhdefo_functions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 01:02:18.509526 akhdefo_functions-2.5.0/akhdefo_functions.egg-info/
--rw-rw-rw-   0        0        0     3935 2024-04-07 01:02:18.000000 akhdefo_functions-2.5.0/akhdefo_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2024-04-07 01:02:18.000000 akhdefo_functions-2.5.0/akhdefo_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 01:02:18.000000 akhdefo_functions-2.5.0/akhdefo_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.0/akhdefo_functions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-04-07 01:02:18.000000 akhdefo_functions-2.5.0/akhdefo_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1236 2024-04-07 00:25:42.000000 akhdefo_functions-2.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 01:02:18.512036 akhdefo_functions-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3617 2024-04-07 00:25:53.000000 akhdefo_functions-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 22:07:06.879460 akhdefo_functions-2.5.1/
+-rw-rw-rw-   0        0        0    10250 2024-04-09 22:07:06.879460 akhdefo_functions-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.1/README.md
+-rw-rw-rw-   0        0        0     8986 2024-04-08 23:21:41.000000 akhdefo_functions-2.5.1/README_pypi.md
+drwxrwxrwx   0        0        0        0 2024-04-09 22:07:06.862402 akhdefo_functions-2.5.1/akhdefo_functions/
+-rw-rw-rw-   0        0        0    53386 2024-04-07 00:24:07.000000 akhdefo_functions-2.5.1/akhdefo_functions/AkhdefoPlot.py
+-rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Classification.py
+-rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Coreg.py
+-rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_GOI.py
+-rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_TS.py
+-rw-rw-rw-   0        0        0    76847 2024-04-06 22:26:04.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Tools.py
+-rw-rw-rw-   0        0        0   153494 2024-04-06 23:34:54.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Utilities.py
+-rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.1/akhdefo_functions/Filter_PreProc.py
+-rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.1/akhdefo_functions/Mosaic_Crop.py
+-rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.1/akhdefo_functions/OpticalFlow.py
+-rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.1/akhdefo_functions/Stacked_Velocity.py
+-rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.1/akhdefo_functions/Unzip_CopyFiles.py
+-rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.1/akhdefo_functions/Video_Streamer.py
+-rw-rw-rw-   0        0        0      683 2024-04-09 18:00:35.000000 akhdefo_functions-2.5.1/akhdefo_functions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 22:07:06.877407 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/
+-rw-rw-rw-   0        0        0    10250 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1236 2024-04-09 18:18:45.000000 akhdefo_functions-2.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 22:07:06.880456 akhdefo_functions-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     3634 2024-04-09 19:57:03.000000 akhdefo_functions-2.5.1/setup.py
```

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/AkhdefoPlot.py` & `akhdefo_functions-2.5.1/akhdefo_functions/AkhdefoPlot.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Classification.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Classification.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Coreg.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Coreg.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_GOI.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_GOI.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_TS.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_TS.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Tools.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Tools.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Akhdefo_Utilities.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Utilities.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Filter_PreProc.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Filter_PreProc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import rasterio
 from rasterio.plot import show
 from skimage import exposure
 import numpy as np
 import cv2
 from rasterio.plot import show_hist
 import matplotlib.pyplot as plt
-import seaborn_image as sea_img
+#import seaborn_image as sea_img
 import os
 from osgeo import gdal
 import numpy as np
 import matplotlib.pyplot as plt
 import numpy as np
 import cv2
 from osgeo import gdal
```

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Mosaic_Crop.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Mosaic_Crop.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/OpticalFlow.py` & `akhdefo_functions-2.5.1/akhdefo_functions/OpticalFlow.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Stacked_Velocity.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Stacked_Velocity.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/Unzip_CopyFiles.py` & `akhdefo_functions-2.5.1/akhdefo_functions/Unzip_CopyFiles.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions/__init__.py` & `akhdefo_functions-2.5.1/akhdefo_functions/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 akhdefo_functions
 
 collection of python modules performs geospatial image processing to moniter land deformation
 """
 
-__version__ = "2.5.0"
+__version__ = "2.5.1"
 __author__ = 'Mahmud Mustafa Muhammad: mahmud.muhamm1@gmail.com'
 __credits__ = 'Simon Fraser university-Department of Earth Sciences'
 
 
 from .AkhdefoPlot import*
 from .Akhdefo_Tools import*
 from .Akhdefo_TS import*
 from .Filter_PreProc import*
 from .Mosaic_Crop import*
 from .OpticalFlow import*
 from .Stacked_Velocity import*
 from .Unzip_CopyFiles import*
 from .Akhdefo_Coreg import*
 from .Akhdefo_Utilities import*
-from .Video_Streamer import*
 from .Akhdefo_Classification import*
 from .Akhdefo_GOI import*
+from .Video_Streamer import*
```

### Comparing `akhdefo_functions-2.5.0/akhdefo_functions.egg-info/SOURCES.txt` & `akhdefo_functions-2.5.1/akhdefo_functions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 README_pypi.md
 pyproject.toml
 setup.py
 ./README_pypi.md
 akhdefo_functions/AkhdefoPlot.py
 akhdefo_functions/Akhdefo_Classification.py
 akhdefo_functions/Akhdefo_Coreg.py
```

### Comparing `akhdefo_functions-2.5.0/pyproject.toml` & `akhdefo_functions-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 
 [project]
 name = "akhdefo_functions"
-version = "2.5.0"
+version = "2.5.1"
 authors = [
   { name="Mahmud Mustafa Muhammad", email="mahmud.muhamm1@gmail.com" },
 ]
 description = "Land Deformation Monitoring Using Optical Satellite Imagery"
 readme = "./README_pypi.md"
 requires-python = ">=3.7"
```

### Comparing `akhdefo_functions-2.5.0/setup.py` & `akhdefo_functions-2.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 # Read the long description from the README file
 with open("./README_pypi.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setup configuration
 setup(
     name='akhdefo_functions',
-    version='2.5.0',
-    description='Land Deformation Monitoring Using Optical Satellite Imagery',
+    version='2.5.1',
+    description='Land Deformation Monitoring Using Optical and SAR Satellite Imagery',
     url='https://github.com/mahmudsfu/AkhDefo',
     author='Mahmud Mustafa Muhammad',
     author_email='mahmud.muhamm1@gmail.com',
     license='Academic Free License (AFL)',
     packages=['akhdefo_functions'],
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -106,9 +106,11 @@
         'Programming Language :: Python :: 3',  
         'Programming Language :: Python :: 3.6',  
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ], 
-    cmdclass=cmdclass
+    cmdclass=cmdclass 
+    
 )
+
```

