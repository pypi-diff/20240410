# Comparing `tmp/ndbioimage-2024.4.3.tar.gz` & `tmp/ndbioimage-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.4.3.tar", max compression
+gzip compressed data, was "ndbioimage-2024.4.4.tar", max compression
```

## Comparing `ndbioimage-2024.4.3.tar` & `ndbioimage-2024.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.3/LICENSE
--rw-r--r--   0        0        0     2608 2023-11-21 15:08:51.110664 ndbioimage-2024.4.3/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.3/ndbioimage/.DS_Store
--rwxr-xr-x   0        0        0    50844 2024-04-03 12:55:00.640967 ndbioimage-2024.4.3/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.3/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.3/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.3/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    28629 2024-04-02 16:23:36.764150 ndbioimage-2024.4.3/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.3/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.3/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6381 2024-03-29 16:56:03.400728 ndbioimage-2024.4.3/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.3/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.3/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.3/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1010 2024-04-03 12:56:06.072918 ndbioimage-2024.4.3/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 ndbioimage-2024.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.4/LICENSE
+-rw-r--r--   0        0        0     2608 2024-04-03 13:37:34.891216 ndbioimage-2024.4.4/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.4/ndbioimage/.DS_Store
+-rwxr-xr-x   0        0        0    50979 2024-04-05 15:20:31.941526 ndbioimage-2024.4.4/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.4/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.4/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.4/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    28629 2024-04-02 16:23:36.764150 ndbioimage-2024.4.4/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.4/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.4/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6381 2024-03-29 16:56:03.400728 ndbioimage-2024.4.4/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.4/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.4/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.4/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1010 2024-04-10 13:19:26.813381 ndbioimage-2024.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 ndbioimage-2024.4.4/PKG-INFO
```

### Comparing `ndbioimage-2024.4.3/LICENSE` & `ndbioimage-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/README.md` & `ndbioimage-2024.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Usage
 
 - Reading an image file and plotting the frame at channel=2, time=1
 
 ```
 import matplotlib.pyplot as plt
 from ndbioimage import Imread
-with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
+with Imread('image_file.tif', axes='ctyx', dtype=int) as im:
     plt.imshow(im[2, 1])
 ```        
         
 - Showing some image metadata
 
 ```
 from ndbioimage import Imread
@@ -37,27 +37,27 @@
     pprint(im)
 ```
 
 - Slicing the image without loading the image into memory
 
 ```
 from ndbioimage import Imread
-with Imread('image_file.tif', axes='cztxy') as im:
+with Imread('image_file.tif', axes='cztyx') as im:
     sliced_im = im[1, :, :, 100:200, 100:200]
 ```
 
 sliced_im is an instance of Imread which will load any image data from file only when needed
 
 
 - Converting (part) of the image to a numpy ndarray
 
 ```
 from ndbioimage import Imread
 import numpy as np
-with Imread('image_file.tif', axes='cztxy') as im:
+with Imread('image_file.tif', axes='cztyx') as im:
     array = np.asarray(im[0, 0])
 ```
 
 ## Adding more formats
 Readers for image formats subclass AbstractReader. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 are required to implement the following methods:
```

### Comparing `ndbioimage-2024.4.3/ndbioimage/.DS_Store` & `ndbioimage-2024.4.4/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/__init__.py` & `ndbioimage-2024.4.4/ndbioimage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,17 +155,18 @@
     def __setitem__(self, path: Path, value: OME) -> None:
         super().__setitem__(self.path_and_lstat(path), value)
 
     def __contains__(self, path: Path) -> bool:
         return super().__contains__(self.path_and_lstat(path))
 
     @staticmethod
-    def path_and_lstat(path: str | Path) -> tuple[Path, Optional[os.stat_result]]:
+    def path_and_lstat(path: str | Path) -> tuple[Path, Optional[os.stat_result], Optional[os.stat_result]]:
         path = Path(path)
-        return path, (path.lstat() if path.exists() else None)
+        return (path, (path.lstat() if path.exists() else None),
+                (path.with_suffix('.ome.xml').lstat() if path.with_suffix('.ome.xml').exists() else None))
 
 
 class Imread(np.lib.mixins.NDArrayOperatorsMixin, ABC):
     """ class to read image files, while taking good care of important metadata,
         currently optimized for .czi files, but can open anything that bioformats can handle
             path: path to the image file
             optional:
```

### Comparing `ndbioimage-2024.4.3/ndbioimage/jvm.py` & `ndbioimage-2024.4.4/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/readers/bfread.py` & `ndbioimage-2024.4.4/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/readers/cziread.py` & `ndbioimage-2024.4.4/ndbioimage/readers/cziread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.4.4/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/readers/ndread.py` & `ndbioimage-2024.4.4/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/readers/seqread.py` & `ndbioimage-2024.4.4/ndbioimage/readers/seqread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/readers/tifread.py` & `ndbioimage-2024.4.4/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/ndbioimage/transforms.py` & `ndbioimage-2024.4.4/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.3/pyproject.toml` & `ndbioimage-2024.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.4.3"
+version = "2024.4.4"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2024.4.3/PKG-INFO` & `ndbioimage-2024.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.8,<4.0
@@ -58,15 +58,15 @@
 ## Usage
 
 - Reading an image file and plotting the frame at channel=2, time=1
 
 ```
 import matplotlib.pyplot as plt
 from ndbioimage import Imread
-with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
+with Imread('image_file.tif', axes='ctyx', dtype=int) as im:
     plt.imshow(im[2, 1])
 ```        
         
 - Showing some image metadata
 
 ```
 from ndbioimage import Imread
@@ -75,27 +75,27 @@
     pprint(im)
 ```
 
 - Slicing the image without loading the image into memory
 
 ```
 from ndbioimage import Imread
-with Imread('image_file.tif', axes='cztxy') as im:
+with Imread('image_file.tif', axes='cztyx') as im:
     sliced_im = im[1, :, :, 100:200, 100:200]
 ```
 
 sliced_im is an instance of Imread which will load any image data from file only when needed
 
 
 - Converting (part) of the image to a numpy ndarray
 
 ```
 from ndbioimage import Imread
 import numpy as np
-with Imread('image_file.tif', axes='cztxy') as im:
+with Imread('image_file.tif', axes='cztyx') as im:
     array = np.asarray(im[0, 0])
 ```
 
 ## Adding more formats
 Readers for image formats subclass AbstractReader. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 are required to implement the following methods:
```

