# Comparing `tmp/clara_viz-0.3.2-py2.py3-none-any.whl.zip` & `tmp/clara_viz-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9822 bytes, number of entries: 8
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-09 11:10 clara/viz/VERSION
+Zip file size: 9818 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-10 08:13 clara/viz/VERSION
 -rw-r--r--  2.0 unx      710 b- defN 24-Mar-22 09:44 clara/viz/__init__.py
 -rw-r--r--  2.0 unx     1626 b- defN 24-Mar-22 09:44 clara/viz/_version.py
--rw-rw-r--  2.0 unx    11419 b- defN 24-Apr-09 11:10 clara_viz-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     7891 b- defN 24-Apr-09 11:10 clara_viz-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-09 11:10 clara_viz-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-09 11:10 clara_viz-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-Apr-09 11:10 clara_viz-0.3.2.dist-info/RECORD
-8 files, 22391 bytes uncompressed, 8736 bytes compressed:  61.0%
+-rw-rw-r--  2.0 unx    11419 b- defN 24-Apr-10 08:13 clara_viz-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7893 b- defN 24-Apr-10 08:13 clara_viz-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-10 08:13 clara_viz-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-10 08:13 clara_viz-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-Apr-10 08:13 clara_viz-0.4.0.dist-info/RECORD
+8 files, 22393 bytes uncompressed, 8732 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: clara/viz/__init__.py
 Comment: 
 
 Filename: clara/viz/_version.py
 Comment: 
 
-Filename: clara_viz-0.3.2.dist-info/LICENSE
+Filename: clara_viz-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: clara_viz-0.3.2.dist-info/METADATA
+Filename: clara_viz-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: clara_viz-0.3.2.dist-info/WHEEL
+Filename: clara_viz-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: clara_viz-0.3.2.dist-info/top_level.txt
+Filename: clara_viz-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: clara_viz-0.3.2.dist-info/RECORD
+Filename: clara_viz-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clara/viz/VERSION

```diff
@@ -1 +1 @@
-0.3.2
+0.4.0
```

## Comparing `clara_viz-0.3.2.dist-info/LICENSE` & `clara_viz-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clara_viz-0.3.2.dist-info/METADATA` & `clara_viz-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clara-viz
-Version: 0.3.2
+Version: 0.4.0
 Summary: A toolkit to provide GPU accelerated visualization of medical data.
 Home-page: https://github.com/NVIDIA/clara-viz
 Author: NVIDIA Corporation
 License: Apache-2.0
 Platform: manylinux_2_28_x86_64
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >= 3.6, <= 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
-Requires-Dist: clara-viz-core (==0.3.2)
-Requires-Dist: clara-viz-widgets (==0.3.2)
+Requires-Dist: clara-viz-core (==0.4.0)
+Requires-Dist: clara-viz-widgets (==0.4.0)
 
 # Quick Start
 
 ## Installation
 
 This will install all Clara Viz packages use pip:
 
@@ -82,15 +82,15 @@
 rgb_data = np.asarray(output)[:, :, :3]
 
 # show with PIL
 image = Image.fromarray(rgb_data)
 image.show()
 ```
 
-# clara-viz 0.3.3 (??? ?? ????)
+# clara-viz 0.4.0 (April 10 2024)
 
 ## Features
 
 * Add Python and pybind11 source code
 * Add support for Python 3.10 and 3.11 packages and set Python wheel requirement to fail installation on unsupported Python versions
 
 ## Bug Fixes
```

