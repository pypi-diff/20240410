# Comparing `tmp/shadow4-advanced-0.0.8.tar.gz` & `tmp/shadow4-advanced-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadow4-advanced-0.0.8.tar", last modified: Fri Feb 23 23:28:18 2024, max compression
+gzip compressed data, was "shadow4-advanced-0.0.9.tar", last modified: Thu Feb 29 20:28:12 2024, max compression
```

## Comparing `shadow4-advanced-0.0.8.tar` & `shadow4-advanced-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:28:18.694262 shadow4-advanced-0.0.8/
--rw-r--r--   0 rook       (505) staff       (20)     1143 2024-02-13 17:33:14.000000 shadow4-advanced-0.0.8/LICENSE
--rw-r--r--   0 rook       (505) staff       (20)      100 2024-02-19 20:42:33.000000 shadow4-advanced-0.0.8/MANIFEST.in
--rw-r--r--   0 rook       (505) staff       (20)      274 2024-02-23 23:28:18.694084 shadow4-advanced-0.0.8/PKG-INFO
--rw-r--r--   0 rook       (505) staff       (20)       64 2024-02-21 01:57:53.000000 shadow4-advanced-0.0.8/README.md
--rw-r--r--   0 rook       (505) staff       (20)       38 2024-02-23 23:28:18.694333 shadow4-advanced-0.0.8/setup.cfg
--rw-r--r--   0 rook       (505) staff       (20)     2716 2024-02-23 23:28:12.000000 shadow4-advanced-0.0.8/setup.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:28:18.692016 shadow4-advanced-0.0.8/shadow4_advanced/
--rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-19 20:25:08.000000 shadow4-advanced-0.0.8/shadow4_advanced/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:28:18.693260 shadow4-advanced-0.0.8/shadow4_advanced/benders/
--rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-19 20:42:14.000000 shadow4-advanced-0.0.8/shadow4_advanced/benders/__init__.py
--rw-r--r--   0 rook       (505) staff       (20)    17765 2024-02-23 23:19:49.000000 shadow4-advanced-0.0.8/shadow4_advanced/benders/s4_flexural_hinge_bender_ellipsoid_mirror.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:28:18.693477 shadow4-advanced-0.0.8/shadow4_advanced/fresnel_zone_plate/
--rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-21 23:10:51.000000 shadow4-advanced-0.0.8/shadow4_advanced/fresnel_zone_plate/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:28:18.693805 shadow4-advanced-0.0.8/shadow4_advanced/hybrid/
--rw-r--r--   0 rook       (505) staff       (20)        0 2024-02-13 17:33:14.000000 shadow4-advanced-0.0.8/shadow4_advanced/hybrid/__init__.py
--rw-r--r--   0 rook       (505) staff       (20)    53117 2024-02-19 22:43:15.000000 shadow4-advanced-0.0.8/shadow4_advanced/hybrid/s4_hybrid_screen.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-23 23:28:18.692908 shadow4-advanced-0.0.8/shadow4_advanced.egg-info/
--rw-r--r--   0 rook       (505) staff       (20)      274 2024-02-23 23:28:18.000000 shadow4-advanced-0.0.8/shadow4_advanced.egg-info/PKG-INFO
--rw-r--r--   0 rook       (505) staff       (20)      501 2024-02-23 23:28:18.000000 shadow4-advanced-0.0.8/shadow4_advanced.egg-info/SOURCES.txt
--rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-23 23:28:18.000000 shadow4-advanced-0.0.8/shadow4_advanced.egg-info/dependency_links.txt
--rw-r--r--   0 rook       (505) staff       (20)      118 2024-02-23 23:28:18.000000 shadow4-advanced-0.0.8/shadow4_advanced.egg-info/requires.txt
--rw-r--r--   0 rook       (505) staff       (20)       17 2024-02-23 23:28:18.000000 shadow4-advanced-0.0.8/shadow4_advanced.egg-info/top_level.txt
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:28:12.520035 shadow4-advanced-0.0.9/
+-rw-r--r--   0 rook       (505) staff       (20)     1143 2024-02-13 17:33:14.000000 shadow4-advanced-0.0.9/LICENSE
+-rw-r--r--   0 rook       (505) staff       (20)      100 2024-02-19 20:42:33.000000 shadow4-advanced-0.0.9/MANIFEST.in
+-rw-r--r--   0 rook       (505) staff       (20)      274 2024-02-29 20:28:12.519823 shadow4-advanced-0.0.9/PKG-INFO
+-rw-r--r--   0 rook       (505) staff       (20)       64 2024-02-21 01:57:53.000000 shadow4-advanced-0.0.9/README.md
+-rw-r--r--   0 rook       (505) staff       (20)       38 2024-02-29 20:28:12.520127 shadow4-advanced-0.0.9/setup.cfg
+-rw-r--r--   0 rook       (505) staff       (20)     2716 2024-02-29 20:28:02.000000 shadow4-advanced-0.0.9/setup.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:28:12.516102 shadow4-advanced-0.0.9/shadow4_advanced/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-19 20:25:08.000000 shadow4-advanced-0.0.9/shadow4_advanced/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:28:12.518027 shadow4-advanced-0.0.9/shadow4_advanced/benders/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-19 20:42:14.000000 shadow4-advanced-0.0.9/shadow4_advanced/benders/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)    19062 2024-02-29 20:09:29.000000 shadow4-advanced-0.0.9/shadow4_advanced/benders/s4_flexural_hinge_bender_ellipsoid_mirror.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:28:12.518334 shadow4-advanced-0.0.9/shadow4_advanced/fresnel_zone_plate/
+-rw-r--r--   0 rook       (505) staff       (20)     3390 2024-02-21 23:10:51.000000 shadow4-advanced-0.0.9/shadow4_advanced/fresnel_zone_plate/__init__.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:28:12.518907 shadow4-advanced-0.0.9/shadow4_advanced/hybrid/
+-rw-r--r--   0 rook       (505) staff       (20)        0 2024-02-13 17:33:14.000000 shadow4-advanced-0.0.9/shadow4_advanced/hybrid/__init__.py
+-rw-r--r--   0 rook       (505) staff       (20)    53117 2024-02-19 22:43:15.000000 shadow4-advanced-0.0.9/shadow4_advanced/hybrid/s4_hybrid_screen.py
+drwxr-xr-x   0 rook       (505) staff       (20)        0 2024-02-29 20:28:12.517417 shadow4-advanced-0.0.9/shadow4_advanced.egg-info/
+-rw-r--r--   0 rook       (505) staff       (20)      274 2024-02-29 20:28:12.000000 shadow4-advanced-0.0.9/shadow4_advanced.egg-info/PKG-INFO
+-rw-r--r--   0 rook       (505) staff       (20)      501 2024-02-29 20:28:12.000000 shadow4-advanced-0.0.9/shadow4_advanced.egg-info/SOURCES.txt
+-rw-r--r--   0 rook       (505) staff       (20)        1 2024-02-29 20:28:12.000000 shadow4-advanced-0.0.9/shadow4_advanced.egg-info/dependency_links.txt
+-rw-r--r--   0 rook       (505) staff       (20)      118 2024-02-29 20:28:12.000000 shadow4-advanced-0.0.9/shadow4_advanced.egg-info/requires.txt
+-rw-r--r--   0 rook       (505) staff       (20)       17 2024-02-29 20:28:12.000000 shadow4-advanced-0.0.9/shadow4_advanced.egg-info/top_level.txt
```

### Comparing `shadow4-advanced-0.0.8/LICENSE` & `shadow4-advanced-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shadow4-advanced-0.0.8/setup.py` & `shadow4-advanced-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,19 +59,19 @@
     'setuptools',
     'numpy',
     'scipy',
     'syned>=1.0.30',
     'srxraylib>=1.0.50',
     'wofryimpl>=1.0.26',
     'shadow4>=0.1.24',
-    'shadow-hybrid-methods>=1.0.7',
+    'shadow-hybrid-methods>=1.0.8',
 )
 
 setup(name='shadow4-advanced',
-      version='0.0.8',
+      version='0.0.9',
       description='advanced tools for shadow4 in python',
       author='Manuel Sanchez del Rio, Luca Rebuffi, Xianbo Shi',
       author_email='lrebuffi@anl.gov',
       url='https://github.com/oasys-kit/shadow4-advanced/',
       packages=PACKAGES,
       install_requires=INSTALL_REQUIRES,
      )
```

### Comparing `shadow4-advanced-0.0.8/shadow4_advanced/__init__.py` & `shadow4-advanced-0.0.9/shadow4_advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `shadow4-advanced-0.0.8/shadow4_advanced/benders/__init__.py` & `shadow4-advanced-0.0.9/shadow4_advanced/benders/__init__.py`

 * *Files identical despite different names*

### Comparing `shadow4-advanced-0.0.8/shadow4_advanced/benders/s4_flexural_hinge_bender_ellipsoid_mirror.py` & `shadow4-advanced-0.0.9/shadow4_advanced/benders/s4_flexural_hinge_bender_ellipsoid_mirror.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 # ----------------------------------------------------------------------- #
 
 from srxraylib.profiles.benders.flexural_hinge_bender_manager import FlexuralHingeStandardBenderManager, FlexuralHingeCalibratedBenderManager, \
     FlexuralHingeBenderStructuralParameters, FlexuralHingeBenderFitParameters, CalibrationParameters, BenderMovement, BenderOuputData, MirrorShape, BenderType
 
 from syned.beamline.shape import EllipticalCylinder, Rectangle
 from syned.beamline.element_coordinates import ElementCoordinates
+from syned.beamline.shape import NumericalMesh
 
 from shadow4.beam.s4_beam import S4Beam
 from shadow4.optical_surfaces.s4_mesh import S4Mesh
 from shadow4.beamline.s4_beamline_element_movements import S4BeamlineElementMovements
 from shadow4.beamline.optical_elements.mirrors.s4_ellipsoid_mirror import S4EllipsoidMirror
 from shadow4.beamline.optical_elements.mirrors.s4_numerical_mesh_mirror import S4NumericalMeshMirror
 from shadow4.beamline.optical_elements.mirrors.s4_additional_numerical_mesh_mirror import S4AdditionalNumericalMeshMirror, S4AdditionalNumericalMeshMirrorElement
@@ -71,15 +72,14 @@
                  ratio=None,
                  bender_shape=MirrorShape.TRAPEZIUM,
                  bender_type= BenderType.DOUBLE_MOMENTUM,
                  calibration_parameters: CalibrationParameters=None,
                  fit_to_focus_parameters: FlexuralHingeBenderFitParameters=None,
                  bender_movement: BenderMovement=None):
         assert ellipsoid_mirror is not None
-
         surface_shape  = ellipsoid_mirror.get_surface_shape()
         boundary_shape = ellipsoid_mirror.get_boundary_shape()
 
         assert not (surface_shape is None and bender_shape is None)
         if not isinstance(surface_shape, EllipticalCylinder): raise ValueError("Calculation is possible on Elliptical Cylinders only")
         if not isinstance(boundary_shape, Rectangle):         raise ValueError("Calculation is possible on Rectangular/Trapezoidal Elliptical Cylinders only")
         assert (bender_bin_x > 0 and bender_bin_y > 0 and E > 0.0 and h > 0.0)
@@ -140,15 +140,15 @@
                                                                                shape=self._bender_shape,
                                                                                bender_type=self._bender_type,
                                                                                workspace_units_to_m=1.0,
                                                                                workspace_units_to_mm=1000.0)
 
         if not fit_to_focus_parameters is None:
             bender_manager = FlexuralHingeStandardBenderManager(bender_structural_parameters=bender_structural_parameters)
-            bender_data = bender_manager.fit_bender_at_focus_position(fit_to_focus_parameters)
+            bender_data = self._bender_manager.fit_bender_at_focus_position(fit_to_focus_parameters)
         elif not bender_movement is None:
             if calibration_parameters is None: bender_manager = FlexuralHingeStandardBenderManager(bender_structural_parameters=bender_structural_parameters)
             else:                              bender_manager = FlexuralHingeCalibratedBenderManager(bender_structural_parameters=bender_structural_parameters, calibration_parameters=calibration_parameters)
 
             bender_data = bender_manager.get_bender_shape_from_movement(bender_movement)
             q           = bender_manager.get_q_ideal_surface(bender_movement)
 
@@ -158,15 +158,41 @@
         S4AdditionalNumericalMeshMirror.__init__(self,
                                                  ideal_mirror=ellipsoid_mirror,
                                                  numerical_mesh_mirror=S4NumericalMeshMirror(boundary_shape=ellipsoid_mirror.get_boundary_shape(),
                                                                                              xx=bender_data.x,
                                                                                              yy=bender_data.y,
                                                                                              zz=bender_data.z_bender_correction.T),
                                                  name=ellipsoid_mirror.get_name())
-        self._bender_data = bender_data
+        self._bender_data      = bender_data
+        self._bender_manager   = bender_manager
+        self._ellipsoid_mirror = ellipsoid_mirror
+
+    def move_bender(self, bender_movement: BenderMovement):
+        if self._bender_movement is None: raise ValueError("This bender has been initialized to fit to focus")
+
+        bender_data = self._bender_manager.get_bender_shape_from_movement(bender_movement)
+        q           = self._bender_manager.get_q_ideal_surface(bender_movement)
+
+        surface_shape  = self._ellipsoid_mirror.get_surface_shape()
+
+        grazing_angle = surface_shape.get_grazing_angle()
+        p, _          = surface_shape.get_p_q(grazing_angle)
+
+        # modification of the shape of the mirror with the average q
+        self._ellipsoid_mirror.get_surface_shape().initialize_from_p_q(p, q, grazing_angle)
+
+        numerical_mesh: NumericalMesh = self.get_surface_shape_instance() # numerical mesh
+        numerical_mesh._xx = bender_data.x
+        numerical_mesh._yy = bender_data.y
+        numerical_mesh._zz = bender_data.z_bender_correction.T
+
+    @property
+    def bender_movement(self) -> BenderMovement: return self._bender_movement
+    @property
+    def calibration_parameters(self) -> CalibrationParameters: return self._calibration_parameters
 
     def get_bender_data(self) -> BenderOuputData: return self._bender_data
 
     def to_python_code(self, **kwargs):
         txt = self.ideal_mirror().to_python_code()
 
         txt += "\n\nfrom shadow4_advanced.benders.s4_flexural_hinge_bender_ellipsoid_mirror import S4FlexuralHingeBenderEllipsoidMirror"
```

### Comparing `shadow4-advanced-0.0.8/shadow4_advanced/fresnel_zone_plate/__init__.py` & `shadow4-advanced-0.0.9/shadow4_advanced/fresnel_zone_plate/__init__.py`

 * *Files identical despite different names*

### Comparing `shadow4-advanced-0.0.8/shadow4_advanced/hybrid/s4_hybrid_screen.py` & `shadow4-advanced-0.0.9/shadow4_advanced/hybrid/s4_hybrid_screen.py`

 * *Files identical despite different names*

