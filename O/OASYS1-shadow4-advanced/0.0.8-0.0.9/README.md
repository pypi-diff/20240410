# Comparing `tmp/OASYS1-shadow4-advanced-0.0.8.tar.gz` & `tmp/OASYS1-shadow4-advanced-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OASYS1-shadow4-advanced-0.0.8.tar", last modified: Fri Feb 23 22:40:34 2024, max compression
+gzip compressed data, was "OASYS1-shadow4-advanced-0.0.9.tar", last modified: Fri Feb 23 23:03:14 2024, max compression
```

## Comparing `OASYS1-shadow4-advanced-0.0.8.tar` & `OASYS1-shadow4-advanced-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 22:40:34.682226 OASYS1-shadow4-advanced-0.0.8/
--rw-r--r--   0 rook       (505) staff       (20)     1096 2024-02-19 19:48:30.000000 OASYS1-shadow4-advanced-0.0.8/LICENSE
--rw-r--r--   0 rook       (505) staff       (20)      188 2024-02-19 20:03:22.000000 OASYS1-shadow4-advanced-0.0.8/MANIFEST.in
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 22:40:34.678391 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/
--rw-r--r--   0 rook       (505) staff       (20)      779 2024-02-23 22:40:34.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/PKG-INFO
--rw-r--r--   0 rook       (505) staff       (20)     1192 2024-02-23 22:40:34.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/SOURCES.txt
--rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-23 22:40:34.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/dependency_links.txt
--rw-r--r--   0 rook       (505) staff       (20)      146 2024-02-23 22:40:34.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/entry_points.txt
--rw-r--r--   0 rook       (505) staff       (20)       84 2024-02-23 22:40:34.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/namespace_packages.txt
--rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-19 19:57:31.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/not-zip-safe
--rw-r--r--   0 rook       (505) staff       (20)       79 2024-02-23 22:40:34.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/requires.txt
--rw-r--r--   0 rook       (505) staff       (20)       14 2024-02-23 22:40:34.000000 OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/top_level.txt
--rw-r--r--   0 rook       (505) staff       (20)      779 2024-02-23 22:40:34.682032 OASYS1-shadow4-advanced-0.0.8/PKG-INFO
--rw-r--r--   0 rook       (505) staff       (20)       53 2024-02-19 19:48:30.000000 OASYS1-shadow4-advanced-0.0.8/README.md
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 22:40:34.678597 OASYS1-shadow4-advanced-0.0.8/orangecontrib/
--rw-r--r--   0 rook       (505) staff       (20)     3445 2024-02-19 19:58:04.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 22:40:34.678854 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/
--rw-r--r--   0 rook       (505) staff       (20)     3445 2024-02-19 19:51:05.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 22:40:34.679074 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/
--rw-r--r--   0 rook       (505) staff       (20)     3445 2024-02-19 19:51:05.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 22:40:34.680127 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/
--rw-r--r--   0 rook       (505) staff       (20)     3533 2024-02-19 20:06:49.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 22:40:34.681719 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/
--rw-r--r--   0 rook       (505) staff       (20)    10570 2024-02-19 20:17:58.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/advanced.png
--rw-r--r--   0 rook       (505) staff       (20)    47447 2022-06-23 16:17:32.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/fixed_rod_bender_mirror.png
--rw-r--r--   0 rook       (505) staff       (20)    40399 2022-06-23 16:17:32.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_mirror.png
--rw-r--r--   0 rook       (505) staff       (20)    26507 2024-02-23 21:20:17.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_scheme.png
--rw-r--r--   0 rook       (505) staff       (20)     4992 2022-06-23 16:14:55.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/hybrid_screen.png
--rw-r--r--   0 rook       (505) staff       (20)    81869 2022-06-23 16:17:32.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/zone_plate.png
--rwxr-xr-x   0 rook       (505) staff       (20)    30378 2024-02-23 22:32:31.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/ow_flexural_hinge_bender_mirror.py
--rw-r--r--   0 rook       (505) staff       (20)    38988 2024-02-21 23:50:55.000000 OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/ow_hybrid_screen.py
--rw-r--r--   0 rook       (505) staff       (20)       38 2024-02-23 22:40:34.682290 OASYS1-shadow4-advanced-0.0.8/setup.cfg
--rwxr-xr-x   0 rook       (505) staff       (20)     4475 2024-02-23 22:40:19.000000 OASYS1-shadow4-advanced-0.0.8/setup.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:03:14.863060 OASYS1-shadow4-advanced-0.0.9/
+-rw-r--r--   0 rook       (505) staff       (20)     1096 2024-02-19 19:48:30.000000 OASYS1-shadow4-advanced-0.0.9/LICENSE
+-rw-r--r--   0 rook       (505) staff       (20)      188 2024-02-19 20:03:22.000000 OASYS1-shadow4-advanced-0.0.9/MANIFEST.in
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:03:14.860109 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/
+-rw-r--r--   0 rook       (505) staff       (20)      779 2024-02-23 23:03:14.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/PKG-INFO
+-rw-r--r--   0 rook       (505) staff       (20)     1192 2024-02-23 23:03:14.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/SOURCES.txt
+-rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-23 23:03:14.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/dependency_links.txt
+-rw-r--r--   0 rook       (505) staff       (20)      146 2024-02-23 23:03:14.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/entry_points.txt
+-rw-r--r--   0 rook       (505) staff       (20)       84 2024-02-23 23:03:14.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/namespace_packages.txt
+-rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-19 19:57:31.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/not-zip-safe
+-rw-r--r--   0 rook       (505) staff       (20)       79 2024-02-23 23:03:14.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/requires.txt
+-rw-r--r--   0 rook       (505) staff       (20)       14 2024-02-23 23:03:14.000000 OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/top_level.txt
+-rw-r--r--   0 rook       (505) staff       (20)      779 2024-02-23 23:03:14.862885 OASYS1-shadow4-advanced-0.0.9/PKG-INFO
+-rw-r--r--   0 rook       (505) staff       (20)       53 2024-02-19 19:48:30.000000 OASYS1-shadow4-advanced-0.0.9/README.md
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:03:14.860279 OASYS1-shadow4-advanced-0.0.9/orangecontrib/
+-rw-r--r--   0 rook       (505) staff       (20)     3445 2024-02-19 19:58:04.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:03:14.860454 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/
+-rw-r--r--   0 rook       (505) staff       (20)     3445 2024-02-19 19:51:05.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:03:14.860622 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/
+-rw-r--r--   0 rook       (505) staff       (20)     3445 2024-02-19 19:51:05.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:03:14.861242 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/
+-rw-r--r--   0 rook       (505) staff       (20)     3533 2024-02-19 20:06:49.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:03:14.862583 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/
+-rw-r--r--   0 rook       (505) staff       (20)    10570 2024-02-19 20:17:58.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/advanced.png
+-rw-r--r--   0 rook       (505) staff       (20)    47447 2022-06-23 16:17:32.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/fixed_rod_bender_mirror.png
+-rw-r--r--   0 rook       (505) staff       (20)    40399 2022-06-23 16:17:32.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_mirror.png
+-rw-r--r--   0 rook       (505) staff       (20)    26507 2024-02-23 21:20:17.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_scheme.png
+-rw-r--r--   0 rook       (505) staff       (20)     4992 2022-06-23 16:14:55.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/hybrid_screen.png
+-rw-r--r--   0 rook       (505) staff       (20)    81869 2022-06-23 16:17:32.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/zone_plate.png
+-rwxr-xr-x   0 rook       (505) staff       (20)    30408 2024-02-23 22:59:13.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/ow_flexural_hinge_bender_mirror.py
+-rw-r--r--   0 rook       (505) staff       (20)    38988 2024-02-21 23:50:55.000000 OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/ow_hybrid_screen.py
+-rw-r--r--   0 rook       (505) staff       (20)       38 2024-02-23 23:03:14.863120 OASYS1-shadow4-advanced-0.0.9/setup.cfg
+-rwxr-xr-x   0 rook       (505) staff       (20)     4475 2024-02-23 23:03:03.000000 OASYS1-shadow4-advanced-0.0.9/setup.py
```

### Comparing `OASYS1-shadow4-advanced-0.0.8/LICENSE` & `OASYS1-shadow4-advanced-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/PKG-INFO` & `OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OASYS1-shadow4-advanced
-Version: 0.0.8
+Version: 0.0.9
 Summary: oasys-shadow4-advanced: Oasys widgets for shadow4 - advanced tools
 Home-page: https://github.com/oasys-kit/OASYS1-SHADOW4-Advanced
 Download-URL: https://github.com/oasys-kit/OASYS1-SHADOW4-Advanced
 Author: M. Sanchez del Rio, L. Rebuffi
 Author-email: lrebuffi@anl.gov
 License: MIT
 Keywords: ray tracing,x-ray optics,Oasys1
```

### Comparing `OASYS1-shadow4-advanced-0.0.8/OASYS1_shadow4_advanced.egg-info/SOURCES.txt` & `OASYS1-shadow4-advanced-0.0.9/OASYS1_shadow4_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/PKG-INFO` & `OASYS1-shadow4-advanced-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OASYS1-shadow4-advanced
-Version: 0.0.8
+Version: 0.0.9
 Summary: oasys-shadow4-advanced: Oasys widgets for shadow4 - advanced tools
 Home-page: https://github.com/oasys-kit/OASYS1-SHADOW4-Advanced
 Download-URL: https://github.com/oasys-kit/OASYS1-SHADOW4-Advanced
 Author: M. Sanchez del Rio, L. Rebuffi
 Author-email: lrebuffi@anl.gov
 License: MIT
 Keywords: ray tracing,x-ray optics,Oasys1
```

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/__init__.py` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/__init__.py` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/__init__.py` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/__init__.py` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/advanced.png` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/advanced.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/fixed_rod_bender_mirror.png` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/fixed_rod_bender_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_mirror.png` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_scheme.png` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/flexural_hinge_bender_scheme.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/hybrid_screen.png` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/hybrid_screen.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/icons/zone_plate.png` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/icons/zone_plate.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/ow_flexural_hinge_bender_mirror.py` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/ow_flexural_hinge_bender_mirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,20 +369,20 @@
     # S4 objects
     #########################################################
 
     def _post_trace_operations(self, output_beam, footprint, element, beamline):
         bender_data = element.get_optical_element().get_bender_data()
 
         if self.use_fitted_result_to_move_bender == 0:
-            self.M1_out = bender_data.M1_out
-            if self.bender_shape==MirrorShape.TRAPEZIUM:     self.e_out     = bender_data.e_out
-            if self.bender_type==BenderType.DOUBLE_MOMENTUM: self.M2_out    = round(bender_data.M1_out * bender_data.ratio_out, 3)
+            self.M1_out = round(bender_data.M1_out, 4)
+            if self.bender_shape==MirrorShape.TRAPEZIUM:     self.e_out     = round(bender_data.e_out, 5)
+            if self.bender_type==BenderType.DOUBLE_MOMENTUM: self.M2_out    = round(bender_data.M1_out * bender_data.ratio_out, 4)
         else:
-            self.M1_movement = bender_data.M1_out
-            if self.bender_type==BenderType.DOUBLE_MOMENTUM: self.M2_movement = round(bender_data.M1_out * bender_data.ratio_out, 3)
+            self.M1_movement = round(bender_data.M1_out, 4)
+            if self.bender_type==BenderType.DOUBLE_MOMENTUM: self.M2_movement = round(bender_data.M1_out * bender_data.ratio_out, 4)
 
             if self.use_calibration==1:
                 def get_q(pos, p0, p1): return round(1/(p0*pos + p1), 6)
 
                 self.q_downstream_movement = get_q(self.pos_downstream, self.p0_downstream, self.p1_downstream)
                 if self.bender_type == BenderType.DOUBLE_MOMENTUM: self.q_upstream_movement = get_q(self.pos_upstream, self.p0_upstream, self.p1_upstream)
```

### Comparing `OASYS1-shadow4-advanced-0.0.8/orangecontrib/shadow4_advanced/widgets/tools/ow_hybrid_screen.py` & `OASYS1-shadow4-advanced-0.0.9/orangecontrib/shadow4_advanced/widgets/tools/ow_hybrid_screen.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-advanced-0.0.8/setup.py` & `OASYS1-shadow4-advanced-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 __license__ = "MIT"
 __date__ = "19/02/2024"
 
 import os
 from setuptools import find_packages, setup
 
 NAME = 'OASYS1-shadow4-advanced'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 ISRELEASED = False
 
 DESCRIPTION = 'oasys-shadow4-advanced: Oasys widgets for shadow4 - advanced tools'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'M. Sanchez del Rio, L. Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
@@ -85,15 +85,15 @@
 SETUP_REQUIRES = (
                   'setuptools',
                   )
 
 INSTALL_REQUIRES = (
                     'oasys1>=1.2.140',
                     'shadow4>=0.1.24',
-                    'shadow4-advanced>=0.0.6',
+                    'shadow4-advanced>=0.0.7',
                     'oasys1-shadow4>=0.0.31',
                     )
 
 PACKAGES = find_packages(exclude=('*.tests', '*.tests.*', 'tests.*', 'tests'))
```

