# Comparing `tmp/PyVecs-0.0.5.tar.gz` & `tmp/PyVecs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVecs-0.0.5.tar", last modified: Sun Feb 18 18:12:43 2024, max compression
+gzip compressed data, was "PyVecs-0.0.6.tar", last modified: Tue Apr  9 22:19:04 2024, max compression
```

## Comparing `PyVecs-0.0.5.tar` & `PyVecs-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 18:12:43.459007 PyVecs-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-18 18:12:43.459007 PyVecs-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 18:12:43.459007 PyVecs-0.0.5/PyVecs/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-18 18:12:35.000000 PyVecs-0.0.5/PyVecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-02-18 18:12:35.000000 PyVecs-0.0.5/PyVecs/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 18:12:43.459007 PyVecs-0.0.5/PyVecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-18 18:12:43.000000 PyVecs-0.0.5/PyVecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-18 18:12:43.000000 PyVecs-0.0.5/PyVecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 18:12:43.000000 PyVecs-0.0.5/PyVecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-18 18:12:43.000000 PyVecs-0.0.5/PyVecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-18 18:12:35.000000 PyVecs-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 18:12:43.459007 PyVecs-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-18 18:12:35.000000 PyVecs-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:04.335529 PyVecs-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 22:19:04.335529 PyVecs-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:04.331529 PyVecs-0.0.6/PyVecs/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 22:18:54.000000 PyVecs-0.0.6/PyVecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-09 22:18:54.000000 PyVecs-0.0.6/PyVecs/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:04.335529 PyVecs-0.0.6/PyVecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 22:18:54.000000 PyVecs-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:19:04.335529 PyVecs-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 22:18:54.000000 PyVecs-0.0.6/setup.py
```

### Comparing `PyVecs-0.0.5/PKG-INFO` & `PyVecs-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: PyVecs
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple 2D and 3D Vector class to Python.
 Author: Thales Rodrigues
 Author-email: thaleshend@gmail.com
 Project-URL: Github, https://github.com/Thales625/PyVecs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10,<=3.12.2
 Description-Content-Type: text/markdown
 
-# Vector
+# PyVecs
 Vector 2D and Vector 3D for Python
+
+## Installation
+
+You can install the library via pip: https://pypi.org/project/PyVecs/
```

### Comparing `PyVecs-0.0.5/PyVecs/main.py` & `PyVecs-0.0.6/PyVecs/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,14 +129,21 @@
     def __pow__(self, other): # Vector2 ^ Scalar
         if is_scalar(other):
             return Vector2(self.x ** other, self.y ** other)
         return None
     
     def __str__(self):
         return f"X: {self.x} Y: {self.y}"
+
+    def clamp(self, _min, _max):
+        if self.x > _max: self.x = _max
+        if self.y > _max: self.y = _max
+
+        if self.x < _min: self.x = _min
+        if self.y < _min: self.y = _min
     
     def rotate(self, theta) -> 'Vector2': # Rotate
         """
         return: a copy of the vector rotated by the specified angle.
         """
         s, c = sin(theta), cos(theta)
         return Vector2(self.x * c - self.y * s, self.x * s + self.y * c)
@@ -284,14 +291,23 @@
         if is_scalar(other):
             return Vector3(self.x ** other, self.y ** other, self.z ** other)
         return None
     
     def __str__(self):
         return f"X: {self.x} Y: {self.y} Z: {self.z}"
     
+    def clamp(self, _min, _max):
+        if self.x > _max: self.x = _max
+        if self.y > _max: self.y = _max
+        if self.z > _max: self.z = _max
+
+        if self.x < _min: self.x = _min
+        if self.y < _min: self.y = _min
+        if self.z < _min: self.z = _min
+    
     def rotateX(self, theta) -> 'Vector3':
         """
         return: a copy of the vector rotated around the x-axis by the specified angle.
         """
         c, s = cos(theta), sin(theta)
         return Vector3(self.x, self.y * c + self.z * s, self.z * c - self.y * s)
```

### Comparing `PyVecs-0.0.5/PyVecs.egg-info/PKG-INFO` & `PyVecs-0.0.6/PyVecs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: PyVecs
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple 2D and 3D Vector class to Python.
 Author: Thales Rodrigues
 Author-email: thaleshend@gmail.com
 Project-URL: Github, https://github.com/Thales625/PyVecs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10,<=3.12.2
 Description-Content-Type: text/markdown
 
-# Vector
+# PyVecs
 Vector 2D and Vector 3D for Python
+
+## Installation
+
+You can install the library via pip: https://pypi.org/project/PyVecs/
```

### Comparing `PyVecs-0.0.5/setup.py` & `PyVecs-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 
 setup(
     name="PyVecs",
-    version="0.0.5",
+    version="0.0.6",
     author="Thales Rodrigues",
     author_email="thaleshend@gmail.com",
     description="A simple 2D and 3D Vector class to Python.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[],
```

