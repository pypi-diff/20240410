# Comparing `tmp/poreanalyser-0.0.3.tar.gz` & `tmp/poreanalyser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poreanalyser-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "poreanalyser-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `poreanalyser-0.0.3.tar` & `poreanalyser-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,50 @@
--rw-r--r--   0        0        0    26526 2024-03-21 20:24:02.841751 poreanalyser-0.0.3/LICENSE
--rw-r--r--   0        0        0     7594 2024-03-21 20:24:02.841751 poreanalyser-0.0.3/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py
--rw-r--r--   0        0        0    28702 2024-03-21 20:24:02.841751 poreanalyser-0.0.3/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py
--rw-r--r--   0        0        0      821 2024-03-21 20:24:02.841751 poreanalyser-0.0.3/PoreAnalyser/__init__.py
--rw-r--r--   0        0        0     3909 2024-03-21 20:24:02.841751 poreanalyser-0.0.3/PoreAnalyser/download_files.py
--rwxr-xr-x   0        0        0  1962791 2024-03-21 20:24:02.853751 poreanalyser-0.0.3/PoreAnalyser/hole2/hole
--rwxr-xr-x   0        0        0    31085 2024-03-21 20:24:02.853751 poreanalyser-0.0.3/PoreAnalyser/hole2/sos_triangle
--rwxr-xr-x   0        0        0  2878646 2024-03-21 20:24:02.865751 poreanalyser-0.0.3/PoreAnalyser/hole2/sph_process
--rw-r--r--   0        0        0     8576 2024-03-21 20:24:02.865751 poreanalyser-0.0.3/PoreAnalyser/hole_analysis.py
--rw-r--r--   0        0        0  1315926 2024-03-21 20:24:02.873751 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9.pdb
--rw-r--r--   0        0        0   294331 2024-03-21 20:24:02.873751 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb
--rw-r--r--   0        0        0  1153849 2024-03-21 20:24:02.877751 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb
--rw-r--r--   0        0        0  1154174 2024-03-21 20:24:02.881751 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb
--rw-r--r--   0        0        0   472405 2024-03-21 20:24:02.885752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb
--rw-r--r--   0        0        0   483623 2024-03-21 20:24:02.885752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb
--rw-r--r--   0        0        0   543505 2024-03-21 20:24:02.889752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb
--rw-r--r--   0        0        0   610576 2024-03-21 20:24:02.889752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb
--rw-r--r--   0        0        0   938821 2024-03-21 20:24:02.893751 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb
--rw-r--r--   0        0        0  1122891 2024-03-21 20:24:02.897752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb
--rw-r--r--   0        0        0   255471 2024-03-21 20:24:02.901752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb
--rw-r--r--   0        0        0   353668 2024-03-21 20:24:02.901752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb
--rw-r--r--   0        0        0  1126446 2024-03-21 20:24:02.905752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb
--rw-r--r--   0        0        0   365834 2024-03-21 20:24:02.909752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb
--rw-r--r--   0        0        0   311491 2024-03-21 20:24:02.909752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb
--rw-r--r--   0        0        0  1126121 2024-03-21 20:24:02.913752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb
--rw-r--r--   0        0        0  1120916 2024-03-21 20:24:02.917752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tvi.pdb
--rw-r--r--   0        0        0  1275076 2024-03-21 20:24:02.921752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1.pdb
--rw-r--r--   0        0        0  1196534 2024-03-21 20:24:02.925752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb
--rw-r--r--   0        0        0  1196859 2024-03-21 20:24:02.933752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb
--rw-r--r--   0        0        0   243451 2024-03-21 20:24:02.933752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb
--rw-r--r--   0        0        0    60805 2024-03-21 20:24:02.933752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.s
--rw-r--r--   0        0        0  1196859 2024-03-21 20:24:02.937752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb
--rw-r--r--   0        0        0  1153849 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb
--rw-r--r--   0        0        0    59106 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph
--rw-r--r--   0        0        0    10727 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/poreanalyser.py
--rw-r--r--   0        0        0      361 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/tests/__init__.py
--rw-r--r--   0        0        0     3372 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/tests/test_ellipse.py
--rw-r--r--   0        0        0     4204 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/tests/test_ellipsoid_optimisation.py
--rw-r--r--   0        0        0     1198 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/tests/test_hole.py
--rw-r--r--   0        0        0      345 2024-03-21 20:24:02.941752 poreanalyser-0.0.3/PoreAnalyser/tests/test_visualization.py
--rw-r--r--   0        0        0    15605 2024-03-21 20:24:02.945752 poreanalyser-0.0.3/PoreAnalyser/visualization.py
--rw-r--r--   0        0        0     4574 2024-03-21 20:24:02.945752 poreanalyser-0.0.3/README.md
--rw-r--r--   0        0        0      763 2024-03-21 20:24:02.945752 poreanalyser-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      321 2024-03-21 20:24:02.945752 poreanalyser-0.0.3/requirements.txt
--rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 poreanalyser-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7594 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py
+-rw-r--r--   0        0        0    28702 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py
+-rw-r--r--   0        0        0      821 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/conductance.py
+-rw-r--r--   0        0        0     3909 2024-04-09 22:27:30.341061 poreanalyser-0.0.4/PoreAnalyser/download_files.py
+-rwxr-xr-x   0        0        0  1962791 2024-04-09 22:27:30.353061 poreanalyser-0.0.4/PoreAnalyser/hole2/hole
+-rwxr-xr-x   0        0        0    31085 2024-04-09 22:27:30.353061 poreanalyser-0.0.4/PoreAnalyser/hole2/sos_triangle
+-rwxr-xr-x   0        0        0  2878646 2024-04-09 22:27:30.365061 poreanalyser-0.0.4/PoreAnalyser/hole2/sph_process
+-rw-r--r--   0        0        0     8576 2024-04-09 22:27:30.365061 poreanalyser-0.0.4/PoreAnalyser/hole_analysis.py
+-rw-r--r--   0        0        0  1315926 2024-04-09 22:27:30.369061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb
+-rw-r--r--   0        0        0   294331 2024-04-09 22:27:30.373061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb
+-rw-r--r--   0        0        0  1153849 2024-04-09 22:27:30.377061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb
+-rw-r--r--   0        0        0  1154174 2024-04-09 22:27:30.381061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb
+-rw-r--r--   0        0        0   472405 2024-04-09 22:27:30.381061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb
+-rw-r--r--   0        0        0   483623 2024-04-09 22:27:30.385061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb
+-rw-r--r--   0        0        0   543505 2024-04-09 22:27:30.389061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb
+-rw-r--r--   0        0        0   610576 2024-04-09 22:27:30.389061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb
+-rw-r--r--   0        0        0   938821 2024-04-09 22:27:30.393061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb
+-rw-r--r--   0        0        0  1122891 2024-04-09 22:27:30.397061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb
+-rw-r--r--   0        0        0   255471 2024-04-09 22:27:30.397061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb
+-rw-r--r--   0        0        0   353668 2024-04-09 22:27:30.401061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb
+-rw-r--r--   0        0        0  1126446 2024-04-09 22:27:30.405061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb
+-rw-r--r--   0        0        0   365834 2024-04-09 22:27:30.405061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb
+-rw-r--r--   0        0        0   311491 2024-04-09 22:27:30.409061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb
+-rw-r--r--   0        0        0    16898 2024-04-09 22:27:30.409061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_pathway_ellipse.txt
+-rw-r--r--   0        0        0  1126121 2024-04-09 22:27:30.413061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb
+-rw-r--r--   0        0        0  1120916 2024-04-09 22:27:30.417061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tvi.pdb
+-rw-r--r--   0        0        0    16497 2024-04-09 22:27:30.417061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tvi_aligned_z.pdb_pathway_ellipse.txt
+-rw-r--r--   0        0        0  1275076 2024-04-09 22:27:30.421061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1.pdb
+-rw-r--r--   0        0        0  1196534 2024-04-09 22:27:30.425061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb
+-rw-r--r--   0        0        0  1196859 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb
+-rw-r--r--   0        0        0   243451 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb
+-rw-r--r--   0        0        0    16047 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_pathway_ellipse.txt
+-rw-r--r--   0        0        0    60805 2024-04-09 22:27:30.433061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.s
+-rw-r--r--   0        0        0  1196859 2024-04-09 22:27:30.437061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb
+-rw-r--r--   0        0        0  1153849 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb
+-rw-r--r--   0        0        0    59106 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph
+-rw-r--r--   0        0        0    16086 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/poreanalyser.py
+-rw-r--r--   0        0        0      361 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/tests/__init__.py
+-rw-r--r--   0        0        0     2251 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/tests/test_conductance.py
+-rw-r--r--   0        0        0     3372 2024-04-09 22:27:30.441061 poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipse.py
+-rw-r--r--   0        0        0     4204 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipsoid_optimisation.py
+-rw-r--r--   0        0        0     1198 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/tests/test_hole.py
+-rw-r--r--   0        0        0      345 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/tests/test_visualization.py
+-rw-r--r--   0        0        0    16323 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/PoreAnalyser/visualization.py
+-rw-r--r--   0        0        0     4765 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/README.md
+-rw-r--r--   0        0        0      764 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      321 2024-04-09 22:27:30.445061 poreanalyser-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     5390 1970-01-01 00:00:00.000000 poreanalyser-0.0.4/PKG-INFO
```

### Comparing `poreanalyser-0.0.3/LICENSE` & `poreanalyser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py` & `poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipse_lib.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py` & `poreanalyser-0.0.4/PoreAnalyser/ProbeParticleEllipsoid/ellipsoid_optimisation.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/__init__.py` & `poreanalyser-0.0.4/PoreAnalyser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 #from .hole_analysis import hole_analysis 
 #sys.path.append('ProbeParticleEllipsoid/')
 #from ellipsoid_optimisation import ellipsoid_optimisation as ellipsoid_analysis 
 #from visualization import write_pdb_with_pore_surface, plt_ellipsoid_pathway, pathway_visu, st_write_ellipsoid, write_pdb_with_ellipsoid_surface, example_xy_plane, compare_volume, render_visu
 #from download_files import download_output, download_Ellipsoid_output
 #from ellipsoid_optimisation import ellipsoid_pathway
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = 'David Seiferth'
 
 from .hole_analysis import hole_analysis
 
 import numpy as np
```

### Comparing `poreanalyser-0.0.3/PoreAnalyser/download_files.py` & `poreanalyser-0.0.4/PoreAnalyser/download_files.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/hole2/hole` & `poreanalyser-0.0.4/PoreAnalyser/hole2/hole`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/hole2/sos_triangle` & `poreanalyser-0.0.4/PoreAnalyser/hole2/sos_triangle`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/hole2/sph_process` & `poreanalyser-0.0.4/PoreAnalyser/hole2/sph_process`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/hole_analysis.py` & `poreanalyser-0.0.4/PoreAnalyser/hole_analysis.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9.pdb_ellipsoid.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb100.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb11.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb12.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb13.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb14.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb24.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb37.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb6.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb8.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb80.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb9.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9_aligned_z.pdb_ellipsoid.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tu9a_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/7tvi.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/7tvi.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb100.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.pdb_ellipsoid.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z.s` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z.s`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/8fe1_aligned_z_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.pdb`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph` & `poreanalyser-0.0.4/PoreAnalyser/pdb_models/test_7tu9_aligned_z.sph`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/tests/test_ellipse.py` & `poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipse.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/tests/test_ellipsoid_optimisation.py` & `poreanalyser-0.0.4/PoreAnalyser/tests/test_ellipsoid_optimisation.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/tests/test_hole.py` & `poreanalyser-0.0.4/PoreAnalyser/tests/test_hole.py`

 * *Files identical despite different names*

### Comparing `poreanalyser-0.0.3/PoreAnalyser/visualization.py` & `poreanalyser-0.0.4/PoreAnalyser/visualization.py`

 * *Files 11% similar despite different names*

```diff
@@ -367,7 +367,15 @@
     ax.set_ylabel("y", fontsize=f_size)
     ax.set_yticklabels([])
     ax.set_xticklabels([])
     ax.set_aspect('equal', adjustable='box')
     plt.gca().set_aspect('equal', adjustable='box')
     fig.tight_layout()
     return fig
+
+def st_write_conductance_estimation(hole1, pf1, hole_c, pf1_c, fig, digits=1 ):
+    st.subheader("Conductance estimation with cylindrical approximation")
+    st.pyplot(fig)
+    st.write('Conductance with conductivity model based on HOLE profile (spherical probe particle) g = ',round(hole_c,digits),' pS')
+    st.write('Conductance with conductivity model based on PoreAnalyser profile (ellipsoidal probe particle) g = ',round(pf1_c,digits),' pS')
+    st.write('Conductance with bulk conductivity based on HOLE profile (spherical probe particle) g = ',round(hole1,digits),' pS')
+    st.write('Conductance with bulk conductivity based on PoreAnalyser profile (ellipsoidal probe particle) g = ',round(pf1,digits),' pS')
```

### Comparing `poreanalyser-0.0.3/README.md` & `poreanalyser-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ---
-title: PoreFinding
+title: PoreAnalyser
 colorFrom: red
 colorTo: green
 sdk: streamlit
 sdk_version: 1.19.0
 app_file: app.py
 pinned: false
-license: mit
+license: LGPL 2.1
 ---
 
-PoreFinding
+PoreAnalyser
 ==============================
 
 [//]: # (Badges)
-[![Documentation Status](https://readthedocs.org/projects/porefinding/badge/?version=latest)](https://porefinding.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/porefinding/badge/?version=latest)](https://porefinding.readthedocs.io/en/latest/?badge=latest) ![License: MIT](https://img.shields.io/badge/License-LGPL_2.1-blue) ![Unittests](https://github.com/DSeiferth/PoreAnalyser/actions/workflows/python-package.yml/badge.svg) ![package](https://github.com/DSeiferth/PoreAnalyser/actions/workflows/python-publish.yml/badge.svg) ![Docker](https://github.com/DSeiferth/PoreAnalyser/actions/workflows/docker-publish.yml/badge.svg)
 
-[Try out this protoype on HugginFace without installing anything](https://huggingface.co/spaces/DSeiferth/PoreFinding_pdb)
+[Try out this software without installing anything](https://poreanalyser.bioch.ox.ac.uk/)
 
 Recent advances in structural biology have led to a growing number of ion channel structures featuring heteromeric subunit assembly, exemplified by synaptic Glycine receptors ([GlyRs](https://www.nature.com/articles/s41467-023-37106-7)) and α4β2 nicotinic receptors. These structures exhibit inherent pore asymmetry, which has raised questions about the role of asymmetry in ion channel function.  Furthermore, molecular dynamics simulations performed on symmetrical homomeric channels often lead to thermal distortion that means conformations of the resulting ensemble are also asymmetrical. We introduce an algorithm that employs ellipsoidal probe particles, enabling a more comprehensive characterization of pore asymmetries. A constriction is more asymmetric for a larger difference between the smaller and larger radius of the ellipsoidal probe particle. 
 
 #### Existing tools for pore pathfinding
 - [HOLE](https://www.holeprogram.org/) uses Monte Carlo simulated annealing procedure to find the best route for a sphere with variable radius to squeeze through the channel.
 - The Channel Annotation Package [CHAP](https://github.com/channotation/chap) combines  calculations of the pore radius, the hydrophobicity of a pore and water density in the pore to predict hydrophobic gates in ion channels.
 - Other tools, such as MOLEonline and CAVER, do not use a probe based algorithm for path finding. Cavities are identified using Voronoi diagrams and molecular surfaces.
@@ -40,30 +40,24 @@
 4. Loop through all spherical probe particles: 
     a) Ellipsoid initialized with spherical probe particle parameters from HOLE output. 
     b) First Nelder-Mead 4-dim optimization to insert ellipsoid with smaller bounds for parameters [x, y, r1, θ ]. 
     c) Second optimization with larger boundaries for parameters to further increase ellipsoid. The loop takes around 60s to complete...
 5. Plot pathway and render pore surface. 
 
 ### Installation
-PoreFinder may be installed as the latest release from PyPI ( pip install PoreFinder ) or in the development version from this github repository. 
+PoreAnalyser may be installed as the latest release from PyPI ( pip install PoreAnalyser ) or in the development version from this github repository. 
 Detailed [installation instructions](https://porefinding.readthedocs.io/en/latest/usage.html#installation) can be found in the documentation.
+After having installed PoreAnalyser locally, you can run the streamlit app yourself: streamlit run app.py
 
 ### Links to documentation
-You can either upload your proteins of interest to the [webservice](https://huggingface.co/spaces/DSeiferth/PoreFinding_pdb) hosted on hugginface
-or you can [install](https://porefinding.readthedocs.io/en/latest/usage.html#installation) the PoreFinding python package on your machine. 
+You can either upload your proteins of interest to the [webservice](https://poreanalyser.bioch.ox.ac.uk/) hosted on a webserver of the Department of Biochemistry (University of Oxford)
+or you can [install](https://porefinding.readthedocs.io/en/latest/usage.html#installation) the PoreAnalyser python package on your machine. 
 If you decide to use the webservice, you can download all output files and visualisation scripts to produce high quality figures. 
 More information about the [output files](https://porefinding.readthedocs.io/en/latest/webservice.html) can be found in the documentation. 
 
 To render 3d representations of the pore surface, you can use a variety of software ranging from py3Dmol, VMD to UCSF Chimera.
 See [Visualisation tools](https://porefinding.readthedocs.io/en/latest/visualisation.html).
 
 
-## Notes
-
-[Hugging Face Spaces](https://huggingface.co/docs/hub/spaces) work as `git` repositories. To keep everything on GitHub but publish on Hugging Face, add the Hugging Face Space repository as a remote repository:
-
-```bash
-git remote add hf https://huggingface.co/spaces/DSeiferth/PoreFinding_pdb
-```
 ## Acknowledgements
-* Rocco Meli for pointing out streamlit and hugginface
+* Rocco Meli for pointing out streamlit (and hugginface)
 * SBCB community for discussion
```

### Comparing `poreanalyser-0.0.3/pyproject.toml` & `poreanalyser-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "PoreAnalyser"
 authors = [{name = "David Seiferth", email = "david.seiferth@oriel.ox.ac.uk"}]
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
-description = "PoreFinding package based on HOLE and MDAnalysis"
-version = "0.0.3"
+description = "PoreAnalyser package based on HOLE and MDAnalysis"
+version = "0.0.4"
 requires-python = ">=3.6"
 dependencies = [
 'numpy >=1.0, <1.23.0',
 'MDAnalysis >=2.0, <3.0',
 'matplotlib>=0.1',
 'pandas>=1.3',
 'streamlit>=1.0',
```

### Comparing `poreanalyser-0.0.3/PKG-INFO` & `poreanalyser-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PoreAnalyser
-Version: 0.0.3
-Summary: PoreFinding package based on HOLE and MDAnalysis
+Version: 0.0.4
+Summary: PoreAnalyser package based on HOLE and MDAnalysis
 Author-email: David Seiferth <david.seiferth@oriel.ox.ac.uk>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy >=1.0, <1.23.0
 Requires-Dist: MDAnalysis >=2.0, <3.0
 Requires-Dist: matplotlib>=0.1
 Requires-Dist: pandas>=1.3
@@ -16,31 +16,31 @@
 Requires-Dist: ipywidgets==7.6.3
 Requires-Dist: scipy
 Requires-Dist: altair<5
 Requires-Dist: nglview
 Requires-Dist: ipython_genutils==0.2.0
 
 ---
-title: PoreFinding
+title: PoreAnalyser
 colorFrom: red
 colorTo: green
 sdk: streamlit
 sdk_version: 1.19.0
 app_file: app.py
 pinned: false
-license: mit
+license: LGPL 2.1
 ---
 
-PoreFinding
+PoreAnalyser
 ==============================
 
 [//]: # (Badges)
-[![Documentation Status](https://readthedocs.org/projects/porefinding/badge/?version=latest)](https://porefinding.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/porefinding/badge/?version=latest)](https://porefinding.readthedocs.io/en/latest/?badge=latest) ![License: MIT](https://img.shields.io/badge/License-LGPL_2.1-blue) ![Unittests](https://github.com/DSeiferth/PoreAnalyser/actions/workflows/python-package.yml/badge.svg) ![package](https://github.com/DSeiferth/PoreAnalyser/actions/workflows/python-publish.yml/badge.svg) ![Docker](https://github.com/DSeiferth/PoreAnalyser/actions/workflows/docker-publish.yml/badge.svg)
 
-[Try out this protoype on HugginFace without installing anything](https://huggingface.co/spaces/DSeiferth/PoreFinding_pdb)
+[Try out this software without installing anything](https://poreanalyser.bioch.ox.ac.uk/)
 
 Recent advances in structural biology have led to a growing number of ion channel structures featuring heteromeric subunit assembly, exemplified by synaptic Glycine receptors ([GlyRs](https://www.nature.com/articles/s41467-023-37106-7)) and α4β2 nicotinic receptors. These structures exhibit inherent pore asymmetry, which has raised questions about the role of asymmetry in ion channel function.  Furthermore, molecular dynamics simulations performed on symmetrical homomeric channels often lead to thermal distortion that means conformations of the resulting ensemble are also asymmetrical. We introduce an algorithm that employs ellipsoidal probe particles, enabling a more comprehensive characterization of pore asymmetries. A constriction is more asymmetric for a larger difference between the smaller and larger radius of the ellipsoidal probe particle. 
 
 #### Existing tools for pore pathfinding
 - [HOLE](https://www.holeprogram.org/) uses Monte Carlo simulated annealing procedure to find the best route for a sphere with variable radius to squeeze through the channel.
 - The Channel Annotation Package [CHAP](https://github.com/channotation/chap) combines  calculations of the pore radius, the hydrophobicity of a pore and water density in the pore to predict hydrophobic gates in ion channels.
 - Other tools, such as MOLEonline and CAVER, do not use a probe based algorithm for path finding. Cavities are identified using Voronoi diagrams and molecular surfaces.
@@ -61,31 +61,25 @@
 4. Loop through all spherical probe particles: 
     a) Ellipsoid initialized with spherical probe particle parameters from HOLE output. 
     b) First Nelder-Mead 4-dim optimization to insert ellipsoid with smaller bounds for parameters [x, y, r1, θ ]. 
     c) Second optimization with larger boundaries for parameters to further increase ellipsoid. The loop takes around 60s to complete...
 5. Plot pathway and render pore surface. 
 
 ### Installation
-PoreFinder may be installed as the latest release from PyPI ( pip install PoreFinder ) or in the development version from this github repository. 
+PoreAnalyser may be installed as the latest release from PyPI ( pip install PoreAnalyser ) or in the development version from this github repository. 
 Detailed [installation instructions](https://porefinding.readthedocs.io/en/latest/usage.html#installation) can be found in the documentation.
+After having installed PoreAnalyser locally, you can run the streamlit app yourself: streamlit run app.py
 
 ### Links to documentation
-You can either upload your proteins of interest to the [webservice](https://huggingface.co/spaces/DSeiferth/PoreFinding_pdb) hosted on hugginface
-or you can [install](https://porefinding.readthedocs.io/en/latest/usage.html#installation) the PoreFinding python package on your machine. 
+You can either upload your proteins of interest to the [webservice](https://poreanalyser.bioch.ox.ac.uk/) hosted on a webserver of the Department of Biochemistry (University of Oxford)
+or you can [install](https://porefinding.readthedocs.io/en/latest/usage.html#installation) the PoreAnalyser python package on your machine. 
 If you decide to use the webservice, you can download all output files and visualisation scripts to produce high quality figures. 
 More information about the [output files](https://porefinding.readthedocs.io/en/latest/webservice.html) can be found in the documentation. 
 
 To render 3d representations of the pore surface, you can use a variety of software ranging from py3Dmol, VMD to UCSF Chimera.
 See [Visualisation tools](https://porefinding.readthedocs.io/en/latest/visualisation.html).
 
 
-## Notes
-
-[Hugging Face Spaces](https://huggingface.co/docs/hub/spaces) work as `git` repositories. To keep everything on GitHub but publish on Hugging Face, add the Hugging Face Space repository as a remote repository:
-
-```bash
-git remote add hf https://huggingface.co/spaces/DSeiferth/PoreFinding_pdb
-```
 ## Acknowledgements
-* Rocco Meli for pointing out streamlit and hugginface
+* Rocco Meli for pointing out streamlit (and hugginface)
 * SBCB community for discussion
```

