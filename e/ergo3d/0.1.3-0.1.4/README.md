# Comparing `tmp/ergo3d-0.1.3.tar.gz` & `tmp/ergo3d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ergo3d-0.1.3.tar", last modified: Fri Apr  5 19:28:18 2024, max compression
+gzip compressed data, was "ergo3d-0.1.4.tar", last modified: Wed Apr 10 03:23:08 2024, max compression
```

## Comparing `ergo3d-0.1.3.tar` & `ergo3d-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 19:28:18.325221 ergo3d-0.1.3/
--rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      467 2024-04-05 19:28:18.324221 ergo3d-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2024-04-02 23:02:10.000000 ergo3d-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 19:28:18.301711 ergo3d-0.1.3/ergo3d/
--rw-rw-rw-   0        0        0       46 2024-04-04 19:41:29.000000 ergo3d-0.1.3/ergo3d/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:28:18.312223 ergo3d-0.1.3/ergo3d/camera/
--rw-rw-rw-   0        0        0     4227 2024-04-05 19:22:21.000000 ergo3d-0.1.3/ergo3d/camera/Camera.py
--rw-rw-rw-   0        0        0    13438 2024-04-02 22:55:21.000000 ergo3d-0.1.3/ergo3d/camera/FLIR_camera.py
--rw-rw-rw-   0        0        0       51 2024-04-04 19:41:29.000000 ergo3d-0.1.3/ergo3d/camera/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:28:18.322222 ergo3d-0.1.3/ergo3d/geometry/
--rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.3/ergo3d/geometry/CoordinateSystem3D.py
--rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.3/ergo3d/geometry/JointAngles.py
--rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.3/ergo3d/geometry/Plane.py
--rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.3/ergo3d/geometry/Point.py
--rw-rw-rw-   0        0        0      105 2024-04-04 19:41:29.000000 ergo3d-0.1.3/ergo3d/geometry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:28:18.307711 ergo3d-0.1.3/ergo3d.egg-info/
--rw-rw-rw-   0        0        0      467 2024-04-05 19:28:18.000000 ergo3d-0.1.3/ergo3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-04-05 19:28:18.000000 ergo3d-0.1.3/ergo3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:28:18.000000 ergo3d-0.1.3/ergo3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 19:28:18.000000 ergo3d-0.1.3/ergo3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 19:28:18.000000 ergo3d-0.1.3/ergo3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 19:28:18.325221 ergo3d-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-05 19:25:25.000000 ergo3d-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.433895 ergo3d-0.1.4/
+-rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-04-10 03:23:08.433895 ergo3d-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2024-04-10 03:22:46.000000 ergo3d-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.417779 ergo3d-0.1.4/ergo3d/
+-rw-rw-rw-   0        0        0       46 2024-04-04 19:41:29.000000 ergo3d-0.1.4/ergo3d/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.425874 ergo3d-0.1.4/ergo3d/camera/
+-rw-rw-rw-   0        0        0     6865 2024-04-09 23:07:34.000000 ergo3d-0.1.4/ergo3d/camera/Camera.py
+-rw-rw-rw-   0        0        0    13438 2024-04-02 22:55:21.000000 ergo3d-0.1.4/ergo3d/camera/FLIR_camera.py
+-rw-rw-rw-   0        0        0       51 2024-04-04 19:41:29.000000 ergo3d-0.1.4/ergo3d/camera/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.433895 ergo3d-0.1.4/ergo3d/geometry/
+-rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/CoordinateSystem3D.py
+-rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/JointAngles.py
+-rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/Plane.py
+-rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/Point.py
+-rw-rw-rw-   0        0        0      105 2024-04-04 19:41:29.000000 ergo3d-0.1.4/ergo3d/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.417779 ergo3d-0.1.4/ergo3d.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:23:08.433895 ergo3d-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-10 03:22:46.000000 ergo3d-0.1.4/setup.py
```

### Comparing `ergo3d-0.1.3/LICENSE` & `ergo3d-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.3/README.md` & `ergo3d-0.1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 
 - `CoordinateSystem3D`: Provides a class for defining 3D coordinate systems.
 
 - `JointAngles`: Provides a class easy ergonomic angle calculations.
 
 ## Installation
 
-### build from source
+### install from PyPI
 ```bash
-git clone https://github.com/LeyangWen/ergo3d.git
-
-
+pip install ergo3d
 ```
 
-### install from PyPI
+### Use from source
 ```bash
-pip install ergo3d
+git clone https://github.com/LeyangWen/ergo3d.git
 ```
 
 ### Steps to update the package on PyPI
 * Update the version number in `setup.py`
 * Build the package and upload to PyPI
 ```bash
 python setup.py sdist bdist_wheel
```

### Comparing `ergo3d-0.1.3/ergo3d/camera/FLIR_camera.py` & `ergo3d-0.1.4/ergo3d/camera/FLIR_camera.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.3/ergo3d/geometry/CoordinateSystem3D.py` & `ergo3d-0.1.4/ergo3d/geometry/CoordinateSystem3D.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.3/ergo3d/geometry/JointAngles.py` & `ergo3d-0.1.4/ergo3d/geometry/JointAngles.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.3/ergo3d/geometry/Plane.py` & `ergo3d-0.1.4/ergo3d/geometry/Plane.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.3/ergo3d/geometry/Point.py` & `ergo3d-0.1.4/ergo3d/geometry/Point.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.3/setup.py` & `ergo3d-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ergo3d',  # Name of your package
-    version='0.1.3',  # Version number
+    version='0.1.4',  # Version number
     description='A Python package for 3D ergonomic calculations.',  # Short description of your package
     url='https://github.com/LeyangWen/ergo3d',  # URL for your package's homepage
     author='Leyang Wen',  # Your name
     author_email='wenleyan@umich.edu',  # Your email
     license='MIT',  # License type for your package
     packages=find_packages(),  # Automatically find all packages and subpackages
     install_requires=[  # List of dependencies
```

