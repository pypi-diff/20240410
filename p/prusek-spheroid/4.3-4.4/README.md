# Comparing `tmp/prusek_spheroid-4.3.tar.gz` & `tmp/prusek_spheroid-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-4.3.tar", last modified: Tue Apr  9 19:04:44 2024, max compression
+gzip compressed data, was "prusek_spheroid-4.4.tar", last modified: Tue Apr  9 19:07:49 2024, max compression
```

## Comparing `prusek_spheroid-4.3.tar` & `prusek_spheroid-4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:04:44.249578 prusek_spheroid-4.3/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-09 19:04:44.249277 prusek_spheroid-4.3/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.3/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:04:44.248013 prusek_spheroid-4.3/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19367 2024-04-09 19:04:24.000000 prusek_spheroid-4.3/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    50417 2024-04-04 18:36:20.000000 prusek_spheroid-4.3/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12428 2024-04-06 18:03:18.000000 prusek_spheroid-4.3/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.3/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.3/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.3/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.3/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.3/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.3/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.3/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.3/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:04:44.249059 prusek_spheroid-4.3/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-09 19:04:44.000000 prusek_spheroid-4.3/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-09 19:04:44.000000 prusek_spheroid-4.3/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-09 19:04:44.000000 prusek_spheroid-4.3/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-09 19:04:44.000000 prusek_spheroid-4.3/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-09 19:04:44.000000 prusek_spheroid-4.3/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-09 19:04:44.249625 prusek_spheroid-4.3/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-09 19:02:49.000000 prusek_spheroid-4.3/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:07:49.047781 prusek_spheroid-4.4/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-09 19:07:49.047565 prusek_spheroid-4.4/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.4/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:07:49.046564 prusek_spheroid-4.4/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-4.4/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    50417 2024-04-04 18:36:20.000000 prusek_spheroid-4.4/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12428 2024-04-06 18:03:18.000000 prusek_spheroid-4.4/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.4/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.4/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.4/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.4/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.4/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.4/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.4/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.4/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:07:49.047362 prusek_spheroid-4.4/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-09 19:07:49.047827 prusek_spheroid-4.4/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-09 19:07:39.000000 prusek_spheroid-4.4/setup.py
```

### Comparing `prusek_spheroid-4.3/PKG-INFO` & `prusek_spheroid-4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.3
+Version: 4.4
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-4.3/README.md` & `prusek_spheroid-4.4/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-4.4/prusek_spheroid/ContoursClassGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 img_gray = cv.resize(img_gray, (1000, 1000), interpolation=cv.INTER_LANCZOS4)
 
                 img_binary, inner_contours_mask = self.apply_segmentation_algorithm(self.algorithm, self.parameters,
                                                                                     img_gray,
                                                                                     self.contours_state)
 
                 outer_contours, _ = cv.findContours(img_binary, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
+                inner_contours = []
                 if self.contours_state == "all" or self.contours_state == "select":
                     inner_contours, _ = cv.findContours(inner_contours_mask, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
                     inner_contours = ip.remove_small_contours(inner_contours)
 
                 height, width = np.shape(img_binary)
 
                 outer_contours = ip.filter_contours_on_frame(outer_contours, (height, width), self.min_area,
```

### Comparing `prusek_spheroid-4.3/prusek_spheroid/GUI.py` & `prusek_spheroid-4.4/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-4.4/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-4.4/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/conversion.py` & `prusek_spheroid-4.4/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/file_management.py` & `prusek_spheroid-4.4/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/image_processing.py` & `prusek_spheroid-4.4/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/merge_directories.py` & `prusek_spheroid-4.4/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/methods.py` & `prusek_spheroid-4.4/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/metrics.py` & `prusek_spheroid-4.4/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-4.4/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-4.4/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.3
+Version: 4.4
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-4.3/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-4.4/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.3/setup.py` & `prusek_spheroid-4.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="4.3",
+    version="4.4",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

